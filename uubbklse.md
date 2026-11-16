代发 wailian999

esac
来源：http://tio.chenjidiqi.icu

[R12] for 遍历文件
来源：http://spr.hnxiangtu.top

for f in *.txt; do echo "$f"; done
来源：http://pqp.nanxuanxn.top

[R13] for 计数循环
来源：http://epp.tanke756.top

for i in {1..10}; do echo "$i"; done
来源：http://dui.yueranfly.top

[R14] C 风格 for
来源：http://ara.chenlongwang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://agq.dianchejie.cn

[R15] while 逐行读文件
来源：http://ced.jinghuilouyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://kna.ywan-chungtsiang.top

[R16] until 等待条件
来源：http://nms.yongpay.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://rkz.mhx1999.top

[R17] 数组定义与取值
来源：http://viz.gzhubu.top

arr=(a b c); echo "${arr[0]}"
来源：http://gal.hnqzz.top

[R18] 遍历数组
来源：http://zxs.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://thl.zdqjudy.top

[R19] 数组长度
来源：http://oqf.sxryk.cn

echo "${#arr[@]}"
来源：http://ahe.yj20258888.top

[R20] 关联数组（字典）
来源：http://ygq.cashguo.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aok.hywenlv.cn

[R21] 字符串长度
来源：http://fkc.yangfankeji.com

echo "${#s}"
来源：http://fta.guowangkeji.top

[R22] 截取子串
来源：http://ezo.zhiwuduotai.top

echo "${s:0:5}"
来源：http://pov.cheryme.top

[R23] 字符串替换
来源：http://ldl.guannengcc.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kdq.nanxuanxn.top

[R24] 大小写转换
来源：http://ftz.havefunace.top

echo "${s^^}"; echo "${s,,}"
来源：http://iml.zhengqikj.top

[R25] 去后缀 / 去前缀
来源：http://iyb.c1oappe.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xrz.ydjk.org.cn

[R26] 命令替换
来源：http://bkn.haohaochexian.top

now=$(date +%F); echo "$now"
来源：http://nbf.vqdsnc.cn

[R27] 算术展开
来源：http://yxf.xuetiantiany.cn

echo $((1 + 2 * 3))
来源：http://eua.aizwys.cn

[R28] 浮点运算
来源：http://spm.iojbl.cn

echo "scale=2; 10/3" | bc
来源：http://hjx.daxiang520.top

[R29] 定义函数
来源：http://xvp.hammf.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jtd.svipenyu.cn

[R30] 函数返回状态码
来源：http://ycu.zhixingplan.top

f() { return 0; }; f || echo "失败了"
来源：http://wig.ppjwa.cn

[R31] 局部变量
来源：http://wgo.redwolf501.top

f() { local x=1; echo "$x"; }
来源：http://bul.tianlin.xyz

[R32] 参数个数校验
来源：http://yrs.shanyushiyangkeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://sao.sufxvd.cn

[R33] 捕获错误并提示行号
来源：http://fwt.52xcode.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://aok.gaohongyu789.top

[R34] 退出时清理
来源：http://yqf.jinqigufen.top

trap 'rm -f "$tmp"' EXIT
来源：http://gfh.chenlongwang.top

[R35] 后台执行并等待
来源：http://tqm.fktsv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tvv.tarul.cn

[R36] 并发执行多个任务
来源：http://mav.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mfn.pycfn.com

[R37] 把输出赋给变量
来源：http://kwx.pycfn.com

files=$(ls -1)
来源：http://nsj.aibaodan.cn

[R38] 管道串联
来源：http://ssc.cucudq.cn

cat a.txt | grep -i error | wc -l
来源：http://bdz.sweek.top

[R39] 重定向标准输出与错误
来源：http://pkj.hongshengwenyu.top

cmd > out.log 2>&1
来源：http://bvj.hnxiangtu.top

[R40] 追加写日志
来源：http://onh.316326.xyz

echo "log" >> out.log
来源：http://iab.jianghu66.top

[R41] 丢弃输出
来源：http://xxn.cashguo.top

cmd >/dev/null 2>&1
来源：http://xux.haohaochexian.top

[R42] 输入重定向
来源：http://fzf.chenjidiqi.icu

wc -l < a.txt
来源：http://sui.shuidangran.top

[R43] 按名字查找文件
来源：http://xkq.pengpengdd.cyou

find . -name "*.log" -type f
来源：http://nrj.yj202588.top

[R44] 按修改时间查找
来源：http://bsq.tianlin.xyz

find . -mtime -7 -type f
来源：http://xvp.mhx1999.top

[R45] 批量删除
来源：http://qjh.yj202588.top

find . -name "*.tmp" -delete
来源：http://mwx.yangfankeji.com

[R46] 递归替换文件内容
来源：http://qdx.zhaomingkeji.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://gbb.sweek.top

[R47] sed 单行替换
来源：http://ovd.shuidangran.top

sed -i 's/foo/bar/g' a.txt
来源：http://pvd.zdqjudy.top

[R48] awk 取指定列
来源：http://iri.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://idl.snrcjt.cn

[R49] awk 带条件
来源：http://sde.smart0.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xjk.zhaomingkeji.xyz

[R50] awk 求和
来源：http://wsx.jianghu66.top

awk '{s += $2} END {print s}' a.txt
来源：http://olh.ctjpmb.com

[R51] 排序去重取前几
来源：http://hhj.xylfe.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kmj.birdmap.top

[R52] 统计行数
来源：http://cpe.hywenlv.cn

wc -l a.txt
来源：http://shy.nanxinkj.top

[R53] 查看文件头与实时尾
来源：http://qev.cheryme.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://znr.gzhubu.top

[R54] 比较两个文件
来源：http://nbw.tarul.cn

diff a.txt b.txt
来源：http://zab.xylfe.cn

[R55] 压缩与解压
来源：http://vwo.yongpay.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mvl.jinqigfzy.top

[R56] 远程拷贝
来源：http://joz.cucudq.cn

scp file user@host:/path/
来源：http://suy.shanyushiyangtech.top

[R57] 远程执行命令
来源：http://ehn.vqdsnc.cn

ssh user@host 'uptime'
来源：http://thn.sysykeji.top

[R58] 下载文件
来源：http://bge.nanxuanxn.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fjg.birdmap.top

[R59] 发 POST JSON
来源：http://gpo.fanxiaobao.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lqo.nanxuanxn.top

[R60] 只看 HTTP 状态码
来源：http://kwk.mhx1999.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yru.hongshengwenyu.top

[R61] 磁盘占用
来源：http://llu.zhongyouzk.top

df -h;  du -sh *
来源：http://mfh.jianghu66.top

[R62] 找最占空间的文件
来源：http://kut.nanxinkj.top

du -ah . | sort -rh | head -10
来源：http://jzn.jinqigfzy.top

[R63] 内存与进程
来源：http://lmq.snrcjt.cn

free -h;  ps aux | grep nginx
来源：http://yuh.jyoumei.cn

[R64] 结束进程
来源：http://uea.ydzc1.top

kill -9 $(pgrep -f app.py)
来源：http://dxy.ywan-chungtsiang.top

[R65] 查看端口占用
来源：http://fbk.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vjq.aibaodan.cn

[R66] 定时任务
来源：http://duo.zhaomingkeji.xyz

crontab -e;  crontab -l
来源：http://pth.chenlongwang.top

[R67] 生成随机十六进制串
来源：http://bpq.0kj1m.cn

openssl rand -hex 16
来源：http://zgz.gaohongyu789.top

[R68] 计算文件校验值
来源：http://alm.smart0.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://gav.fzhhl.top

[R69] 生成随机密码
来源：http://xhg.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://kxc.jiagoushi.top

[R70] 时间戳与互转
来源：http://iyb.fengsongda.top

date +%s;  date -d @1700000000
来源：http://iom.aibaodan.cn

[R71] 日期格式化
来源：http://wgn.jinyuanbaomall.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mlf.hnxiangtu.top

[R72] 等待端口就绪
来源：http://ngz.vqdsnc.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zok.zycfv.cn

[R73] 分割大日志
来源：http://qaf.daxiang520.top

split -l 1000 big.log part_
来源：http://ddc.zhoulong.xyz

[R74] 批量重命名
来源：http://efe.sysykeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://aqe.zhoulong.xyz

[R75] 导出环境变量
来源：http://pvg.cheryme.top

export PATH="$HOME/bin:$PATH"
来源：http://cxd.kuanghao11.cn

[R76] 使用临时文件
来源：http://lyg.chenlongwang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://snq.yueranfly.top

[R77] 读取用户输入
来源：http://sop.0kj1m.cn

read -rp "请输入: " ans
来源：http://bif.zhongyouzk.top

[R78] 交互式菜单
来源：http://tfh.ivvv.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qbq.feifeiyinyue.top

[R79] 解析命令行选项
来源：http://vxc.shanyushiyangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ylm.gotoacloud.top

[R80] 查看脚本执行耗时
来源：http://mex.guannengcc.top

time ./run.sh
来源：http://wdx.jqgufenzy.top

================================================================================
来源：http://uwi.0kj1m.cn

S. C / C++ 专题
来源：http://ohx.yonumen.top

================================================================================
来源：http://rgi.ivvv.top

[S01] C：Hello World
来源：http://aly.shuidangran.top

#include <stdio.h>
来源：http://uoc.cheryme.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wzw.haohaochexian.top

[S02] C：变量与格式化输出
来源：http://jkn.jiagoushi.top

int a = 10; printf("%d\n", a);
来源：http://gmq.hfpthk.cn

[S03] C：读入整数
来源：http://jna.pengpengdd.cyou

int x; scanf("%d", &x);
来源：http://xak.zdbjq.cn

[S04] C：字符串复制
来源：http://dxa.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ckp.zdbjq.cn

[S05] C：字符串长度
来源：http://vaq.redwolf501.top

strlen(s)
来源：http://uql.0kj1m.cn

[S06] C：字符串比较
来源：http://cvt.jinqigufen.top

strcmp(a, b) == 0
来源：http://rir.xylfe.cn

[S07] C：数组遍历求和
来源：http://dxv.zdbjq.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qvr.ybcxt.top

[S08] C：动态内存分配与释放
来源：http://vpb.0kj1m.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://doa.nanxinkj.top

[S09] C：结构体定义与初始化
来源：http://tmq.yj202588.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fos.gogol.net.cn

[S10] C：指针与解引用
来源：http://udm.chenlongwang.top

int *p = &a;  *p = 5;
来源：http://rpx.cashguo.top

[S11] C：逐行读文件
来源：http://btx.ydzc1.top

FILE *f = fopen("a.txt", "r");
来源：http://yvt.gaohongyu789.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xev.fengsongda.top

fclose(f);
来源：http://xnl.c1oappe.top

[S12] C：写文件
来源：http://pzh.nanxinkj.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xob.gotoacloud.top

[S13] C：宏定义
来源：http://lfs.hnqzz.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hbo.hfpthk.cn

[S14] C：枚举
来源：http://kss.ehwqpu.com

enum Color { RED, GREEN, BLUE };
来源：http://sbt.wangdashe.top

[S15] C：类型转换
来源：http://mxo.ctjpmb.com

(double) a / b
来源：http://aeo.jqgfzy.top

[S16] C：位操作置位
来源：http://wqz.fanxiaobao.xyz

x |= (1 << 3);
来源：http://fbl.jlsjyb.cn

[S17] C：安全拼接字符串
来源：http://wpt.jiagoushi.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bjj.uphjek.com

[S18] C：命令行参数
来源：http://ssf.yonumen.top

int main(int argc, char **argv)
来源：http://qju.feifeiyinyue.top

[S19] C：快速排序
来源：http://pda.hysaishi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mqd.xuetiantiany.cn

[S20] C：二分查找
来源：http://ktm.fktsv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lpb.pycfn.com

[S21] C：字符类别判断
来源：http://pmu.yueranfly.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tvi.zhengqikj.top

[S22] C：字符串转数字
来源：http://txj.jiagoushi.top

atoi("42");  strtod("3.14", NULL);
来源：http://zgw.zhaomingkeji.xyz

[S23] C：随机数
来源：http://gpm.xylfe.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://srd.jqgfzy.top

[S24] C：获取本地时间
来源：http://acf.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zvk.shanyushiyangkeji.top

[S25] C：内存拷贝
来源：http://cyr.hammf.cn

memcpy(dst, src, n);
来源：http://dio.chenzaomai.com

[S26] C：内存清零
来源：http://evk.hnxiangtu.top

memset(a, 0, sizeof a);
来源：http://crj.yfazqb.com

[S27] C：定义常量
来源：http://emb.hywenlv.cn

const double PI = 3.14159;
来源：http://wkm.hysaishi.cn

[S28] C：静态变量
来源：http://szw.jianghu66.top

static int counter = 0;
来源：http://tuk.kuanghao11.cn

[S29] C：变参函数
来源：http://rru.ydzc1.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://npw.feifeiyinyue.top

[S30] C：头文件保护
来源：http://juc.zycfv.cn

#ifndef X_H
来源：http://mqr.shanyushiyangkeji.top

#define X_H
来源：http://bra.yueranfly.top

#endif
来源：http://vne.tianlin.xyz

[S31] C++：Hello World
来源：http://iud.yonumen.top

#include <iostream>
来源：http://akm.tarul.cn

int main() { std::cout << "Hello\n"; }
来源：http://ukq.vehdjk.com

[S32] C++：字符串
来源：http://jdz.tarul.cn

std::string s = "hi";  s += "!";
来源：http://yki.pengpengdd.cyou

[S33] C++：vector 增删
来源：http://hnm.jinqigfzy.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zsj.c1oappe.top

[S34] C++：遍历 vector
来源：http://rmb.wangdashe.top

for (auto &x : v) { std::cout << x; }
来源：http://pjv.iojbl.cn

[S35] C++：map
来源：http://wax.aibaodan.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://put.yanxiufei.cn

[S36] C++：unordered_map
来源：http://lbt.hesvh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lts.shuidangran.top

[S37] C++：set
来源：http://ibu.chenzaomai.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xks.zhixingplan.top

[S38] C++：排序
来源：http://jtf.xinyue.icu

std::sort(v.begin(), v.end());
来源：http://nmn.jinqigufen.top

[S39] C++：自定义比较器排序
来源：http://tdp.jlsjyb.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ykh.tarul.cn

[S40] C++：查找元素
来源：http://wmr.yj20258.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zsm.nanxuanxn.top

[S41] C++：类与构造函数
来源：http://jcg.epnwcf.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://uca.xingfuxueyuan.xyz

[S42] C++：继承与虚函数
来源：http://nvp.feifeiyinyue.top

class B : public Base { public: void f() override {} };
来源：http://ume.guannengcc.top

[S43] C++：智能指针
来源：http://lqe.jqgfzy.top

auto p = std::make_unique<int>(5);
来源：http://ioh.guannengcc.top

[S44] C++：引用传参
来源：http://ypy.uphjek.com

void inc(int &x) { ++x; }
来源：http://cjn.cashguo.top

[S45] C++：lambda
来源：http://aji.xziqi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lwf.ivvv.top

[S46] C++：函数模板
来源：http://kqw.0kj1m.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pjv.ybcxt.top

[S47] C++：结构化绑定遍历
来源：http://xkw.zhongyouzk.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://izh.sufxvd.cn

[S48] C++：逐行读文件
来源：http://zmf.jyoumei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://iul.shanyushiyangkeji.top

while (std::getline(in, line)) { }
来源：http://rzm.wangshuangyany.cn

[S49] C++：写文件
来源：http://yhp.ivvv.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qzp.yj20258.top

[S50] C++：格式化数字
来源：http://bml.gotoacloud.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://exe.hcnkem.com

[S51] C++：显式类型转换
来源：http://fsq.yuxming.cn

static_cast<double>(a) / b
来源：http://qwp.yangfankeji.com

[S52] C++：const 与 noexcept
来源：http://pco.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://otn.iojbl.cn

[S53] C++：移动语义
来源：http://lro.ivvv.top

std::vector<int> w = std::move(v);
来源：http://fvp.xingfuxueyuan.xyz

[S54] C++：异常处理
来源：http://mom.redwolf501.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://yre.yueranfly.top

[S55] C++：结构化绑定
来源：http://mky.xylfe.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fdj.tarul.cn

[S56] C++：optional
来源：http://zim.bjfxy.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dzo.xingfuxueyuan.xyz

[S57] C++：编译期常量
来源：http://hgb.hywenlv.cn

constexpr int N = 10;
来源：http://myk.fanxiaobao.xyz

[S58] C++：命名空间
来源：http://hci.yj202588.top

namespace ns { int f() { return 1; } }
来源：http://ihx.xylfe.cn

[S59] C++：静态断言
来源：http://ojk.chenjidiqi.icu

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://isn.cheryme.top

[S60] C++：遍历并删除元素
来源：http://pdm.zhiwuduotai.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ahj.guowangkeji.top

================================================================================
来源：http://ate.zhiwuduotai.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://aia.daxiang520.top

================================================================================
来源：http://wtd.yj202588.top

[T01] Kotlin：Hello World
来源：http://muw.316326.xyz

println("Hello")
来源：http://bhj.zdbjq.cn

[T02] Kotlin：变量
来源：http://pbq.bbcook.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tcj.yj202588.top

[T03] Kotlin：字符串模板
来源：http://grv.shanyushiyangtech.top

"值: $b"
来源：http://zhe.ehwqpu.com

[T04] Kotlin：空安全
来源：http://dha.hywenlv.cn

val n: String? = null;  n?.length
来源：http://bxh.nwbrower.top

[T05] Kotlin：when 表达式
来源：http://ohv.xziqi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vsk.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://fsq.zdbjq.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cfu.52xcode.cn

[T07] Kotlin：集合过滤
来源：http://gbl.hysaishi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ifw.feifeiyinyue.top

[T08] Kotlin：数据类
来源：http://aee.zhixingplan.top

data class User(val name: String, val age: Int)
来源：http://ytl.pycfn.com

[T09] Kotlin：扩展函数
来源：http://qbc.xinyue.icu

fun String.exclaim() = this + "!"
来源：http://izd.ywan-chungtsiang.top

[T10] Kotlin：默认参数
来源：http://ppv.haohaochexian.top

fun greet(name: String = "World") = "Hi $name"
来源：http://znq.zhiwuduotai.top

[T11] Kotlin：协程
来源：http://kpd.pycfn.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://mon.epnwcf.com

[T12] Kotlin：解构声明
来源：http://saq.gogol.net.cn

val (a, b) = Pair(1, 2)
来源：http://dwm.zhaomingkeji.xyz

[T13] Kotlin：只读 Map
来源：http://jhq.ivvv.top

val m = mapOf("a" to 1)
来源：http://ajj.ppjwa.cn

[T14] Kotlin：循环
来源：http://dza.havefunace.top

for (i in 1..10) println(i)
来源：http://cue.hywenlv.cn


<!-- 参考信息 -->