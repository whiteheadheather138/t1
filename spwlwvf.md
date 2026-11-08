代发 wailian999

name="${1:-default}"
来源：https://sf.zhonguo3118.cn

[R06] 判断命令是否存在
来源：https://jd.zhonguo3118.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：https://nq.zhonguo7118.cn

[R07] if 判断文件
来源：https://ie.zhonguo4118.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：https://oy.zhonguo3118.cn

[R08] 数值比较
来源：https://qk.zhonguo3118.cn

if (( a > b )); then echo "a 更大"; fi
来源：https://wb.zhonguo4118.cn

[R09] 字符串比较
来源：https://vz.zhonguo2118.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：https://gy.zhonguo6118.cn

[R10] 正则匹配
来源：https://fu.zhonguo7118.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：https://wl.zhonguo2118.cn

[R11] case 多分支
来源：https://ux.zhonguo6118.cn

case "$1" in
来源：https://hs.zhonguo5118.cn

start) echo "启动" ;;
来源：https://uu.zhonguo2118.cn

stop)  echo "停止" ;;
来源：https://om.zhonguo3118.cn

*)     echo "未知命令" ;;
来源：https://lt.zhonguo8118.cn

esac
来源：https://vp.zhonguo4118.cn

[R12] for 遍历文件
来源：https://ui.zhonguo5118.cn

for f in *.txt; do echo "$f"; done
来源：https://gh.zhonguo5118.cn

[R13] for 计数循环
来源：https://qu.zhonguo7118.cn

for i in {1..10}; do echo "$i"; done
来源：https://ni.zhonguo2118.cn

[R14] C 风格 for
来源：https://zf.zhonguo6118.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：https://yv.zhonguo6118.cn

[R15] while 逐行读文件
来源：https://mz.zhonguo2118.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：https://bq.zhonguo7118.cn

[R16] until 等待条件
来源：https://za.zhonguo7118.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：https://xx.zhonguo6118.cn

[R17] 数组定义与取值
来源：https://ie.zhonguo1118.cn

arr=(a b c); echo "${arr[0]}"
来源：https://rx.zhonguo8118.cn

[R18] 遍历数组
来源：https://rf.zhonguo1118.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：https://dk.zhonguo3118.cn

[R19] 数组长度
来源：https://lz.zhonguo2118.cn

echo "${#arr[@]}"
来源：https://pf.zhonguo3118.cn

[R20] 关联数组（字典）
来源：https://yz.zhonguo7118.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：https://dj.zhonguo2118.cn

[R21] 字符串长度
来源：https://lt.zhonguo3118.cn

echo "${#s}"
来源：https://zx.zhonguo3118.cn

[R22] 截取子串
来源：https://hi.zhonguo2118.cn

echo "${s:0:5}"
来源：https://ys.zhonguo6118.cn

[R23] 字符串替换
来源：https://te.zhonguo4118.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：https://hj.zhonguo1118.cn

[R24] 大小写转换
来源：https://km.zhonguo7118.cn

echo "${s^^}"; echo "${s,,}"
来源：https://wm.zhonguo2118.cn

[R25] 去后缀 / 去前缀
来源：https://yd.zhonguo4118.cn

echo "${f%.txt}"; echo "${f#./}"
来源：https://kp.zhonguo7118.cn

[R26] 命令替换
来源：https://tx.zhonguo1118.cn

now=$(date +%F); echo "$now"
来源：https://pl.zhonguo8118.cn

[R27] 算术展开
来源：https://py.zhonguo7118.cn

echo $((1 + 2 * 3))
来源：https://xa.zhonguo8118.cn

[R28] 浮点运算
来源：https://vv.zhonguo6118.cn

echo "scale=2; 10/3" | bc
来源：https://rh.zhonguo2118.cn

[R29] 定义函数
来源：https://ra.zhonguo8118.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：https://ud.zhonguo7118.cn

[R30] 函数返回状态码
来源：https://sd.zhonguo2118.cn

f() { return 0; }; f || echo "失败了"
来源：https://mx.zhonguo7118.cn

[R31] 局部变量
来源：https://ws.zhonguo5118.cn

f() { local x=1; echo "$x"; }
来源：https://dl.zhonguo6118.cn

[R32] 参数个数校验
来源：https://on.zhonguo3118.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：https://vs.zhonguo7118.cn

[R33] 捕获错误并提示行号
来源：https://nm.zhonguo5118.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：https://zu.zhonguo5118.cn

[R34] 退出时清理
来源：https://wx.zhonguo5118.cn

trap 'rm -f "$tmp"' EXIT
来源：https://oa.zhonguo2118.cn

[R35] 后台执行并等待
来源：https://vk.zhonguo6118.cn

sleep 5 & pid=$!; wait "$pid"
来源：https://vs.zhonguo3118.cn

[R36] 并发执行多个任务
来源：https://eu.zhonguo6118.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：https://kj.zhonguo7118.cn

[R37] 把输出赋给变量
来源：https://ao.zhonguo8118.cn

files=$(ls -1)
来源：https://xb.zhonguo3118.cn

[R38] 管道串联
来源：https://fv.zhonguo1118.cn

cat a.txt | grep -i error | wc -l
来源：https://kn.zhonguo6118.cn

[R39] 重定向标准输出与错误
来源：https://jn.zhonguo1118.cn

cmd > out.log 2>&1
来源：https://vm.zhonguo2118.cn

[R40] 追加写日志
来源：https://iw.zhonguo2118.cn

echo "log" >> out.log
来源：https://xd.zhonguo1118.cn

[R41] 丢弃输出
来源：https://eu.zhonguo3118.cn

cmd >/dev/null 2>&1
来源：https://qp.zhonguo7118.cn

[R42] 输入重定向
来源：https://uz.zhonguo5118.cn

wc -l < a.txt
来源：https://ri.zhonguo2118.cn

[R43] 按名字查找文件
来源：https://du.zhonguo5118.cn

find . -name "*.log" -type f
来源：https://vy.zhonguo2118.cn

[R44] 按修改时间查找
来源：https://yx.zhonguo2118.cn

find . -mtime -7 -type f
来源：https://hz.zhonguo8118.cn

[R45] 批量删除
来源：https://pt.zhonguo1118.cn

find . -name "*.tmp" -delete
来源：https://td.zhonguo1118.cn

[R46] 递归替换文件内容
来源：https://bf.zhonguo4118.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：https://mj.zhonguo6118.cn

[R47] sed 单行替换
来源：https://zs.zhonguo8118.cn

sed -i 's/foo/bar/g' a.txt
来源：https://fl.zhonguo3118.cn

[R48] awk 取指定列
来源：https://yr.zhonguo3118.cn

awk '{print $1, $3}' a.txt
来源：https://mz.zhonguo4118.cn

[R49] awk 带条件
来源：https://vw.zhonguo8118.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：https://tt.zhonguo2118.cn

[R50] awk 求和
来源：https://hf.zhonguo6118.cn

awk '{s += $2} END {print s}' a.txt
来源：https://dh.zhonguo1118.cn

[R51] 排序去重取前几
来源：https://lj.zhonguo5118.cn

sort a.txt | uniq -c | sort -rn | head
来源：https://dw.zhonguo1118.cn

[R52] 统计行数
来源：https://ew.zhonguo5118.cn

wc -l a.txt
来源：https://aa.zhonguo6118.cn

[R53] 查看文件头与实时尾
来源：https://ps.zhonguo8118.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：https://cg.zhonguo6118.cn

[R54] 比较两个文件
来源：https://iq.zhonguo4118.cn

diff a.txt b.txt
来源：https://cv.zhonguo4118.cn

[R55] 压缩与解压
来源：https://gg.zhonguo3118.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：https://jf.zhonguo8118.cn

[R56] 远程拷贝
来源：https://ta.zhonguo3118.cn

scp file user@host:/path/
来源：https://pr.zhonguo7118.cn

[R57] 远程执行命令
来源：https://tn.zhonguo4118.cn

ssh user@host 'uptime'
来源：https://hw.zhonguo2118.cn

[R58] 下载文件
来源：https://py.zhonguo8118.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：https://ya.zhonguo5118.cn

[R59] 发 POST JSON
来源：https://fp.zhonguo6118.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：https://fw.zhonguo2118.cn

[R60] 只看 HTTP 状态码
来源：https://gw.zhonguo5118.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：https://bk.zhonguo6118.cn

[R61] 磁盘占用
来源：https://od.zhonguo4118.cn

df -h;  du -sh *
来源：https://or.zhonguo7118.cn

[R62] 找最占空间的文件
来源：https://qk.zhonguo5118.cn

du -ah . | sort -rh | head -10
来源：https://mt.zhonguo5118.cn

[R63] 内存与进程
来源：https://hs.zhonguo6118.cn

free -h;  ps aux | grep nginx
来源：https://wd.zhonguo5118.cn

[R64] 结束进程
来源：https://nu.zhonguo2118.cn

kill -9 $(pgrep -f app.py)
来源：https://vs.zhonguo7118.cn

[R65] 查看端口占用
来源：https://av.zhonguo1118.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：https://wx.zhonguo3118.cn

[R66] 定时任务
来源：https://je.zhonguo5118.cn

crontab -e;  crontab -l
来源：https://ep.zhonguo3118.cn

[R67] 生成随机十六进制串
来源：https://pi.zhonguo4118.cn

openssl rand -hex 16
来源：https://lx.zhonguo8118.cn

[R68] 计算文件校验值
来源：https://mz.zhonguo6118.cn

sha256sum a.txt;  md5sum a.txt
来源：https://aa.zhonguo6118.cn

[R69] 生成随机密码
来源：https://zm.zhonguo4118.cn

head -c 16 /dev/urandom | base64
来源：https://ve.zhonguo3118.cn

[R70] 时间戳与互转
来源：https://zt.zhonguo6118.cn

date +%s;  date -d @1700000000
来源：https://cy.zhonguo5118.cn

[R71] 日期格式化
来源：https://vk.zhonguo3118.cn

date +"%Y-%m-%d %H:%M:%S"
来源：https://ry.zhonguo2118.cn

[R72] 等待端口就绪
来源：https://go.zhonguo4118.cn

until nc -z localhost 3306; do sleep 1; done
来源：https://hx.zhonguo8118.cn

[R73] 分割大日志
来源：https://qv.zhonguo1118.cn

split -l 1000 big.log part_
来源：https://ec.zhonguo5118.cn

[R74] 批量重命名
来源：https://nk.zhonguo2118.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：https://ld.zhonguo4118.cn

[R75] 导出环境变量
来源：https://qo.zhonguo1118.cn

export PATH="$HOME/bin:$PATH"
来源：https://sv.zhonguo5118.cn

[R76] 使用临时文件
来源：https://ss.zhonguo8118.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：https://ni.zhonguo3118.cn

[R77] 读取用户输入
来源：https://uy.zhonguo6118.cn

read -rp "请输入: " ans
来源：https://kh.zhonguo1118.cn

[R78] 交互式菜单
来源：https://jt.zhonguo7118.cn

select opt in a b c; do echo "$opt"; break; done
来源：https://px.zhonguo8118.cn

[R79] 解析命令行选项
来源：https://jm.zhonguo5118.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：https://tv.zhonguo5118.cn

[R80] 查看脚本执行耗时
来源：https://oq.zhonguo3118.cn

time ./run.sh
来源：https://ph.zhonguo4118.cn

================================================================================
来源：https://bz.zhonguo7118.cn

S. C / C++ 专题
来源：https://wq.zhonguo2118.cn

================================================================================
来源：https://td.zhonguo1118.cn

[S01] C：Hello World
来源：https://xy.zhonguo2118.cn

#include <stdio.h>
来源：https://rj.zhonguo4118.cn

int main(void) { printf("Hello\n"); return 0; }
来源：https://wr.zhonguo8118.cn

[S02] C：变量与格式化输出
来源：https://yh.zhonguo4118.cn

int a = 10; printf("%d\n", a);
来源：https://rz.zhonguo8118.cn

[S03] C：读入整数
来源：https://km.zhonguo5118.cn

int x; scanf("%d", &x);
来源：https://ie.zhonguo7118.cn

[S04] C：字符串复制
来源：https://gg.zhonguo3118.cn

char dst[32]; strcpy(dst, "hi");
来源：https://ar.zhonguo3118.cn

[S05] C：字符串长度
来源：https://hy.zhonguo8118.cn

strlen(s)
来源：https://yt.zhonguo8118.cn

[S06] C：字符串比较
来源：https://qk.zhonguo8118.cn

strcmp(a, b) == 0
来源：https://sr.zhonguo8118.cn

[S07] C：数组遍历求和
来源：https://nz.zhonguo5118.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：https://dq.zhonguo3118.cn

[S08] C：动态内存分配与释放
来源：https://rn.zhonguo7118.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：https://xj.zhonguo4118.cn

[S09] C：结构体定义与初始化
来源：https://op.zhonguo2118.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：https://vu.zhonguo4118.cn

[S10] C：指针与解引用
来源：https://ny.zhonguo8118.cn

int *p = &a;  *p = 5;
来源：https://ln.zhonguo1118.cn

[S11] C：逐行读文件
来源：https://rl.zhonguo2118.cn

FILE *f = fopen("a.txt", "r");
来源：https://hh.zhonguo8118.cn

while (fgets(buf, sizeof buf, f)) { }
来源：https://ix.zhonguo2118.cn

fclose(f);
来源：https://ha.zhonguo1118.cn

[S12] C：写文件
来源：https://wx.zhonguo7118.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：https://oz.zhonguo8118.cn

[S13] C：宏定义
来源：https://zj.zhonguo8118.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：https://gc.zhonguo4118.cn

[S14] C：枚举
来源：https://xv.zhonguo8118.cn

enum Color { RED, GREEN, BLUE };
来源：https://if.zhonguo2118.cn

[S15] C：类型转换
来源：https://dd.zhonguo6118.cn

(double) a / b
来源：https://lz.zhonguo8118.cn

[S16] C：位操作置位
来源：https://gd.zhonguo7118.cn

x |= (1 << 3);
来源：https://cn.zhonguo5118.cn

[S17] C：安全拼接字符串
来源：https://uz.zhonguo5118.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：https://eh.zhonguo8118.cn

[S18] C：命令行参数
来源：https://iu.zhonguo4118.cn

int main(int argc, char **argv)
来源：https://ic.zhonguo3118.cn

[S19] C：快速排序
来源：https://ii.zhonguo6118.cn

qsort(a, n, sizeof(int), cmp);
来源：https://qf.zhonguo7118.cn

[S20] C：二分查找
来源：https://my.zhonguo7118.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：https://ah.zhonguo8118.cn

[S21] C：字符类别判断
来源：https://pj.zhonguo7118.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：https://cl.zhonguo4118.cn

[S22] C：字符串转数字
来源：https://ju.zhonguo4118.cn

atoi("42");  strtod("3.14", NULL);
来源：https://zb.zhonguo7118.cn

[S23] C：随机数
来源：https://ha.zhonguo1118.cn

srand(time(NULL));  int r = rand() % 100;
来源：https://ed.zhonguo2118.cn

[S24] C：获取本地时间
来源：https://wl.zhonguo7118.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：https://em.zhonguo3118.cn

[S25] C：内存拷贝
来源：https://vd.zhonguo1118.cn

memcpy(dst, src, n);
来源：https://km.zhonguo1118.cn

[S26] C：内存清零
来源：https://er.zhonguo6118.cn

memset(a, 0, sizeof a);
来源：https://eu.zhonguo4118.cn

[S27] C：定义常量
来源：https://op.zhonguo8118.cn

const double PI = 3.14159;
来源：https://ag.zhonguo5118.cn

[S28] C：静态变量
来源：https://bt.zhonguo3118.cn

static int counter = 0;
来源：https://rh.zhonguo1118.cn

[S29] C：变参函数
来源：https://co.zhonguo4118.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：https://wl.zhonguo1118.cn

[S30] C：头文件保护
来源：https://km.zhonguo3118.cn

#ifndef X_H
来源：https://ni.zhonguo4118.cn

#define X_H
来源：https://nb.zhonguo8118.cn

#endif
来源：https://jw.zhonguo3118.cn

[S31] C++：Hello World
来源：https://gm.zhonguo4118.cn

#include <iostream>
来源：https://am.zhonguo6118.cn

int main() { std::cout << "Hello\n"; }
来源：https://qm.zhonguo3118.cn

[S32] C++：字符串
来源：https://iw.zhonguo3118.cn

std::string s = "hi";  s += "!";
来源：https://ku.zhonguo3118.cn

[S33] C++：vector 增删
来源：https://ee.zhonguo3118.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：https://ss.zhonguo4118.cn

[S34] C++：遍历 vector
来源：https://mj.zhonguo1118.cn

for (auto &x : v) { std::cout << x; }
来源：https://wv.zhonguo1118.cn

[S35] C++：map
来源：https://wt.zhonguo4118.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：https://am.zhonguo4118.cn

[S36] C++：unordered_map
来源：https://oz.zhonguo8118.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：https://th.zhonguo1118.cn

[S37] C++：set
来源：https://fu.zhonguo6118.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：https://no.zhonguo6118.cn

[S38] C++：排序
来源：https://ri.zhonguo2118.cn

std::sort(v.begin(), v.end());
来源：https://fb.zhonguo2118.cn

[S39] C++：自定义比较器排序
来源：https://ps.zhonguo7118.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：https://tc.zhonguo4118.cn

[S40] C++：查找元素
来源：https://wa.zhonguo4118.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：https://sc.zhonguo8118.cn

[S41] C++：类与构造函数
来源：https://eh.zhonguo8118.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：https://xc.zhonguo5118.cn

[S42] C++：继承与虚函数
来源：https://bj.zhonguo5118.cn

class B : public Base { public: void f() override {} };
来源：https://dn.zhonguo8118.cn

[S43] C++：智能指针
来源：https://wl.zhonguo5118.cn

auto p = std::make_unique<int>(5);
来源：https://yj.zhonguo5118.cn

[S44] C++：引用传参
来源：https://rq.zhonguo1118.cn

void inc(int &x) { ++x; }
来源：https://tb.zhonguo1118.cn

[S45] C++：lambda
来源：https://jz.zhonguo4118.cn

auto add = [](int a, int b) { return a + b; };
来源：https://va.zhonguo5118.cn

[S46] C++：函数模板
来源：https://jm.zhonguo5118.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：https://qi.zhonguo4118.cn

[S47] C++：结构化绑定遍历
来源：https://pz.zhonguo8118.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：https://vp.zhonguo7118.cn

[S48] C++：逐行读文件
来源：https://xk.zhonguo6118.cn

std::ifstream in("a.txt");  std::string line;
来源：https://wq.zhonguo7118.cn

while (std::getline(in, line)) { }
来源：https://ej.zhonguo7118.cn

[S49] C++：写文件
来源：https://dw.zhonguo5118.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：https://ac.zhonguo5118.cn

[S50] C++：格式化数字
来源：https://mz.zhonguo1118.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：https://eh.zhonguo1118.cn

[S51] C++：显式类型转换
来源：https://gw.zhonguo4118.cn

static_cast<double>(a) / b
来源：https://or.zhonguo2118.cn

[S52] C++：const 与 noexcept
来源：https://dh.zhonguo8118.cn

int size() const noexcept { return n_; }
来源：https://zp.zhonguo4118.cn

[S53] C++：移动语义
来源：https://sa.zhonguo2118.cn

std::vector<int> w = std::move(v);
来源：https://kk.zhonguo7118.cn

[S54] C++：异常处理
来源：https://hb.zhonguo1118.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：https://uw.zhonguo1118.cn

[S55] C++：结构化绑定
来源：https://fs.zhonguo5118.cn

auto [a, b] = std::make_pair(1, 2);
来源：https://lc.zhonguo8118.cn

[S56] C++：optional
来源：https://kt.zhonguo3118.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：https://ju.zhonguo8118.cn

[S57] C++：编译期常量
来源：https://yl.zhonguo3118.cn

constexpr int N = 10;
来源：https://nc.zhonguo3118.cn

[S58] C++：命名空间
来源：https://cl.zhonguo1118.cn

namespace ns { int f() { return 1; } }
来源：https://py.zhonguo3118.cn

[S59] C++：静态断言
来源：https://kw.zhonguo2118.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：https://jn.zhonguo7118.cn

[S60] C++：遍历并删除元素
来源：https://wp.zhonguo8118.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：https://xe.zhonguo2118.cn

================================================================================
来源：https://jb.zhonguo6118.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：https://sm.zhonguo3118.cn

================================================================================
来源：https://bs.zhonguo7118.cn

[T01] Kotlin：Hello World
来源：https://bz.zhonguo5118.cn

println("Hello")
来源：https://xd.zhonguo5118.cn

[T02] Kotlin：变量
来源：https://oh.zhonguo4118.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：https://kp.zhonguo8118.cn

[T03] Kotlin：字符串模板
来源：https://ba.zhonguo3118.cn

"值: $b"
来源：https://ev.zhonguo2118.cn

[T04] Kotlin：空安全
来源：https://mj.zhonguo2118.cn

val n: String? = null;  n?.length
来源：https://ob.zhonguo1118.cn

[T05] Kotlin：when 表达式
来源：https://kz.zhonguo3118.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：https://ez.zhonguo4118.cn

[T06] Kotlin：集合映射
来源：https://ib.zhonguo5118.cn

listOf(1, 2, 3).map { it * 2 }
来源：https://gx.zhonguo7118.cn


<!-- 参考信息 -->