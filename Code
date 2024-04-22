// Produto escalar usando alocação dinâmica
#include <stdio.h>
#include <stdlib.h>

// Protótipo da função que cria um vetor
int *criaVetor(int n);

// Protótipo da função que calcula o produto escalar
int produtoEscalar(int *v1, int *v2, int n);

// Função principal
int main(void){
  int n;
  int *v1, *v2, vp;
  int produto;

  scanf("%d\n", &n);

  v1 = criaVetor(n);
  v2 = criaVetor(n);

  vp = produtoEscalar(v1, v2, n);

  printf("%d\n", vp);
}

// Função que cria um vetor
int *criaVetor(int n){
  int *v;
  int i;
  v = (int *) malloc(n * sizeof(int));
  for(i = 0; i < n; i++){
    scanf("%d", &v[i]);
  }
  return v;
}

// Função que calcula o produto escalar
int produtoEscalar(int *v1, int *v2, int n){
  int res;
  int i;
  res = 0;
  for(i = 0; i < n; i++){
    res += v1[i] * v2[i];
  }
  return res;
}
