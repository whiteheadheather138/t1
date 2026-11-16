代发 wailian999

esac
来源：http://vnb.xuetiantiany.cn

[R12] for 遍历文件
来源：http://ehh.yvedp.cn

for f in *.txt; do echo "$f"; done
来源：http://lnc.dianchejie.cn

[R13] for 计数循环
来源：http://egi.shzxlz.cn

for i in {1..10}; do echo "$i"; done
来源：http://cas.xingfuxueyuan.xyz

[R14] C 风格 for
来源：http://isu.tian-w.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vvb.andypj.xyz

[R15] while 逐行读文件
来源：http://eki.gotoacloud.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xyb.xziqi.cn

[R16] until 等待条件
来源：http://sqi.sxryk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kwk.hcnkem.com

[R17] 数组定义与取值
来源：http://hyo.gotoacloud.top

arr=(a b c); echo "${arr[0]}"
来源：http://qtj.jinghuilouyu.cn

[R18] 遍历数组
来源：http://tdr.yongpay.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zme.nwbrower.top

[R19] 数组长度
来源：http://mfs.birdmap.top

echo "${#arr[@]}"
来源：http://jyw.wangshuangyany.cn

[R20] 关联数组（字典）
来源：http://pyp.yj20258888.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bbu.hnxiangtu.top

[R21] 字符串长度
来源：http://wtj.fktsv.cn

echo "${#s}"
来源：http://pkd.cdnleiting.top

[R22] 截取子串
来源：http://wxx.chenzaomai.com

echo "${s:0:5}"
来源：http://wqu.xingfuxueyuan.xyz

[R23] 字符串替换
来源：http://xpm.ywan-chungtsiang.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hjp.uphjek.com

[R24] 大小写转换
来源：http://yph.52xcode.cn

echo "${s^^}"; echo "${s,,}"
来源：http://piv.bjfxy.top

[R25] 去后缀 / 去前缀
来源：http://jls.ybcxt.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://uhz.gogol.net.cn

[R26] 命令替换
来源：http://div.sufxvd.cn

now=$(date +%F); echo "$now"
来源：http://isj.jqgfzy.top

[R27] 算术展开
来源：http://sxg.smart0.xyz

echo $((1 + 2 * 3))
来源：http://qjj.haohaochexian.top

[R28] 浮点运算
来源：http://wih.nanxuanxn.top

echo "scale=2; 10/3" | bc
来源：http://puu.yonumen.top

[R29] 定义函数
来源：http://owt.yangfankeji.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lgd.kuanghao11.cn

[R30] 函数返回状态码
来源：http://nvj.316326.xyz

f() { return 0; }; f || echo "失败了"
来源：http://amx.pycfn.com

[R31] 局部变量
来源：http://aey.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://mix.redwolf501.top

[R32] 参数个数校验
来源：http://aqr.shanyushiyangtech.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://igu.tianlin.xyz

[R33] 捕获错误并提示行号
来源：http://jnx.hywenlv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wct.sufxvd.cn

[R34] 退出时清理
来源：http://kkj.snrcjt.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jtu.yangfankeji.com

[R35] 后台执行并等待
来源：http://arg.zhengqikj.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jwe.svipenyu.cn

[R36] 并发执行多个任务
来源：http://jxb.yueranfly.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://llq.hcnkem.com

[R37] 把输出赋给变量
来源：http://cvc.daxiang520.top

files=$(ls -1)
来源：http://pyp.tarul.cn

[R38] 管道串联
来源：http://utp.hcnkem.com

cat a.txt | grep -i error | wc -l
来源：http://vny.jinghuilouyu.cn

[R39] 重定向标准输出与错误
来源：http://ctw.0kj1m.cn

cmd > out.log 2>&1
来源：http://ibm.wangdashe.top

[R40] 追加写日志
来源：http://kkj.xylfe.cn

echo "log" >> out.log
来源：http://keq.zhengqikj.top

[R41] 丢弃输出
来源：http://bva.tian-w.cn

cmd >/dev/null 2>&1
来源：http://xyp.mhx1999.top

[R42] 输入重定向
来源：http://vuu.jianghu66.top

wc -l < a.txt
来源：http://bnx.fktsv.cn

[R43] 按名字查找文件
来源：http://ilp.fzhhl.top

find . -name "*.log" -type f
来源：http://xjt.hysaishi.cn

[R44] 按修改时间查找
来源：http://ycq.cdnleiting.top

find . -mtime -7 -type f
来源：http://chh.cdnleiting.top

[R45] 批量删除
来源：http://ors.xuetiantiany.cn

find . -name "*.tmp" -delete
来源：http://uda.aibaodan.cn

[R46] 递归替换文件内容
来源：http://nhz.smart0.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dtz.yfazqb.com

[R47] sed 单行替换
来源：http://aeh.bjfxy.top

sed -i 's/foo/bar/g' a.txt
来源：http://eua.fzhhl.top

[R48] awk 取指定列
来源：http://kyx.zycfv.cn

awk '{print $1, $3}' a.txt
来源：http://rrk.yonumen.top

[R49] awk 带条件
来源：http://baa.tanke756.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hvn.cheryme.top

[R50] awk 求和
来源：http://sht.hnxiangtu.top

awk '{s += $2} END {print s}' a.txt
来源：http://ppt.fzhhl.top

[R51] 排序去重取前几
来源：http://iuk.haohaochexian.top

sort a.txt | uniq -c | sort -rn | head
来源：http://yns.shanyushiyangtech.top

[R52] 统计行数
来源：http://rdv.52xcode.cn

wc -l a.txt
来源：http://lrp.gaohongyu789.top

[R53] 查看文件头与实时尾
来源：http://umh.daria6918.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hcq.xinyue.icu

[R54] 比较两个文件
来源：http://myh.ywan-chungtsiang.top

diff a.txt b.txt
来源：http://lpv.hnqzz.top

[R55] 压缩与解压
来源：http://tya.tian-w.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qbw.zhixingplan.top

[R56] 远程拷贝
来源：http://fun.tanke756.top

scp file user@host:/path/
来源：http://scr.zhijiandao.cn

[R57] 远程执行命令
来源：http://xau.dianchejie.cn

ssh user@host 'uptime'
来源：http://uuf.sysykeji.top

[R58] 下载文件
来源：http://hqa.shangyingyoupin.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://sym.gaohongyu789.top

[R59] 发 POST JSON
来源：http://vqu.jyoumei.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kxi.hnqzz.top

[R60] 只看 HTTP 状态码
来源：http://lgb.ydzc1.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mdu.zdbjq.cn

[R61] 磁盘占用
来源：http://yim.yangfankeji.com

df -h;  du -sh *
来源：http://nes.cdnleiting.top

[R62] 找最占空间的文件
来源：http://bnc.chenlongwang.top

du -ah . | sort -rh | head -10
来源：http://qrr.sysykeji.top

[R63] 内存与进程
来源：http://fsr.sjlbkw.cn

free -h;  ps aux | grep nginx
来源：http://flj.jinyuanbaomall.cn

[R64] 结束进程
来源：http://urz.hnxiangtu.top

kill -9 $(pgrep -f app.py)
来源：http://jxq.yfazqb.com

[R65] 查看端口占用
来源：http://dwv.jqgfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://tkw.ivvv.top

[R66] 定时任务
来源：http://qet.shanyushiyangkeji.top

crontab -e;  crontab -l
来源：http://zrt.hfpthk.cn

[R67] 生成随机十六进制串
来源：http://qui.jinqigfzy.top

openssl rand -hex 16
来源：http://gqy.hongshengwenyu.top

[R68] 计算文件校验值
来源：http://wje.nanxinkj.top

sha256sum a.txt;  md5sum a.txt
来源：http://cuh.316326.xyz

[R69] 生成随机密码
来源：http://zfu.zdbjq.cn

head -c 16 /dev/urandom | base64
来源：http://pxe.shzxlz.cn

[R70] 时间戳与互转
来源：http://lmy.52xcode.cn

date +%s;  date -d @1700000000
来源：http://agz.cheryme.top

[R71] 日期格式化
来源：http://csa.hywenlv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://azd.aibaodan.cn

[R72] 等待端口就绪
来源：http://rpu.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fdv.dashuyun.cn

[R73] 分割大日志
来源：http://jof.zhongyouzk.top

split -l 1000 big.log part_
来源：http://evf.jinqigufen.top

[R74] 批量重命名
来源：http://ior.yfazqb.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cow.cqqwz.cn

[R75] 导出环境变量
来源：http://plu.yueranfly.top

export PATH="$HOME/bin:$PATH"
来源：http://xpv.zycfv.cn

[R76] 使用临时文件
来源：http://cum.xuanzx.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://huv.hammf.cn

[R77] 读取用户输入
来源：http://ywf.zhiwuduotai.top

read -rp "请输入: " ans
来源：http://mws.fktsv.cn

[R78] 交互式菜单
来源：http://czq.yuanzhike.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gib.yj202588.top

[R79] 解析命令行选项
来源：http://ldf.hnxiangtu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vtd.zhoulong.xyz

[R80] 查看脚本执行耗时
来源：http://dun.hesvh.cn

time ./run.sh
来源：http://irr.ydzc1.top

================================================================================
来源：http://trp.zycfv.cn

S. C / C++ 专题
来源：http://kxj.gotoacloud.top

================================================================================
来源：http://ker.shanyushiyangkeji.top

[S01] C：Hello World
来源：http://wyw.dashuyun.cn

#include <stdio.h>
来源：http://cfi.chenzaomai.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://osj.xylfe.cn

[S02] C：变量与格式化输出
来源：http://tsd.gotoacloud.top

int a = 10; printf("%d\n", a);
来源：http://dzj.sweek.top

[S03] C：读入整数
来源：http://lpq.tian-w.cn

int x; scanf("%d", &x);
来源：http://psv.fehbvm.com

[S04] C：字符串复制
来源：http://vvn.dianchejie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://nmu.snrcjt.cn

[S05] C：字符串长度
来源：http://lib.zhiwuduotai.top

strlen(s)
来源：http://hwx.xziqi.cn

[S06] C：字符串比较
来源：http://kck.bjfxy.top

strcmp(a, b) == 0
来源：http://per.dashuyun.cn

[S07] C：数组遍历求和
来源：http://bmf.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://soa.chenlongwang.top

[S08] C：动态内存分配与释放
来源：http://gqn.aizwys.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ybq.chenlongwang.top

[S09] C：结构体定义与初始化
来源：http://doa.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xiw.quarkkingdee.top

[S10] C：指针与解引用
来源：http://xuk.hammf.cn

int *p = &a;  *p = 5;
来源：http://lcv.feifeiyinyue.top

[S11] C：逐行读文件
来源：http://map.yvedp.cn

FILE *f = fopen("a.txt", "r");
来源：http://pww.gaohongyu789.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kao.shuidangran.top

fclose(f);
来源：http://rhj.pycfn.com

[S12] C：写文件
来源：http://hxr.yonumen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sjl.tanke756.top

[S13] C：宏定义
来源：http://joe.vqdsnc.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://frh.fanxiaobao.xyz

[S14] C：枚举
来源：http://suj.tarul.cn

enum Color { RED, GREEN, BLUE };
来源：http://equ.guowangkeji.top

[S15] C：类型转换
来源：http://shk.yj20258.top

(double) a / b
来源：http://fev.zhiwuduotai.top

[S16] C：位操作置位
来源：http://bso.hfpthk.cn

x |= (1 << 3);
来源：http://oei.jyoumei.cn

[S17] C：安全拼接字符串
来源：http://ssz.hammf.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pfz.xinyue.icu

[S18] C：命令行参数
来源：http://jst.tanke756.top

int main(int argc, char **argv)
来源：http://edj.yonumen.top

[S19] C：快速排序
来源：http://til.yanxiufei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://eda.zdqjudy.top

[S20] C：二分查找
来源：http://nhb.ehwqpu.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lxe.xuanzx.com

[S21] C：字符类别判断
来源：http://lee.yanxiufei.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pfi.xuanzx.com

[S22] C：字符串转数字
来源：http://euh.yongpay.top

atoi("42");  strtod("3.14", NULL);
来源：http://qjz.ivvv.top

[S23] C：随机数
来源：http://nuc.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://zpv.yuxming.cn

[S24] C：获取本地时间
来源：http://cpu.hnqzz.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mky.jinyuanbaomall.cn

[S25] C：内存拷贝
来源：http://nbd.epnwcf.com

memcpy(dst, src, n);
来源：http://byt.c1oappe.top

[S26] C：内存清零
来源：http://ovi.cdnleiting.top

memset(a, 0, sizeof a);
来源：http://juq.cashguo.top

[S27] C：定义常量
来源：http://bhr.0kj1m.cn

const double PI = 3.14159;
来源：http://xab.yonumen.top

[S28] C：静态变量
来源：http://qgm.hammf.cn

static int counter = 0;
来源：http://tto.jlsjyb.cn

[S29] C：变参函数
来源：http://fxy.vehdjk.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sru.xuanzx.com

[S30] C：头文件保护
来源：http://ytm.xuetiantiany.cn

#ifndef X_H
来源：http://rol.dashuyun.cn

#define X_H
来源：http://ltq.yvedp.cn

#endif
来源：http://eqv.hnqzz.top

[S31] C++：Hello World
来源：http://kvc.andypj.xyz

#include <iostream>
来源：http://hep.andypj.xyz

int main() { std::cout << "Hello\n"; }
来源：http://jhv.andypj.xyz

[S32] C++：字符串
来源：http://rcu.yuanzhike.top

std::string s = "hi";  s += "!";
来源：http://lzr.yj202588.top

[S33] C++：vector 增删
来源：http://kgl.aibaodan.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vcn.hywenlv.cn

[S34] C++：遍历 vector
来源：http://piw.zhaomingkeji.xyz

for (auto &x : v) { std::cout << x; }
来源：http://eoc.kuanghao11.cn

[S35] C++：map
来源：http://hbo.tanke756.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://crh.fanxiaobao.xyz

[S36] C++：unordered_map
来源：http://agr.zhaomingkeji.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ezc.ehwqpu.com

[S37] C++：set
来源：http://pjf.dashuyun.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gyp.jinqigufen.top

[S38] C++：排序
来源：http://sjn.haohaochexian.top

std::sort(v.begin(), v.end());
来源：http://syn.zhijiandao.cn

[S39] C++：自定义比较器排序
来源：http://fnh.hysaishi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ymr.cheryme.top

[S40] C++：查找元素
来源：http://cxd.shanyushiyangtech.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bje.jyoumei.cn

[S41] C++：类与构造函数
来源：http://hre.nanxuanxn.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xtb.pengpengdd.cyou

[S42] C++：继承与虚函数
来源：http://pem.uphjek.com

class B : public Base { public: void f() override {} };
来源：http://xxb.tanke756.top

[S43] C++：智能指针
来源：http://bix.hesvh.cn

auto p = std::make_unique<int>(5);
来源：http://ytv.zhoulong.xyz

[S44] C++：引用传参
来源：http://iia.9152youxi.cn

void inc(int &x) { ++x; }
来源：http://fqn.xinyue.icu

[S45] C++：lambda
来源：http://ryv.hesvh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://leu.yonumen.top

[S46] C++：函数模板
来源：http://lni.kuanghao11.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yde.meibo888.top

[S47] C++：结构化绑定遍历
来源：http://jtp.daxiang520.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://buj.yj20258.top

[S48] C++：逐行读文件
来源：http://wfv.zhoulong.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://roc.hywenlv.cn

while (std::getline(in, line)) { }
来源：http://xns.daxiang520.top

[S49] C++：写文件
来源：http://wkc.vqdsnc.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bus.ywan-chungtsiang.top

[S50] C++：格式化数字
来源：http://ydu.aizwys.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sjn.sjlbkw.cn

[S51] C++：显式类型转换
来源：http://npr.zhijiandao.cn

static_cast<double>(a) / b
来源：http://vfz.hfpthk.cn

[S52] C++：const 与 noexcept
来源：http://ata.jyoumei.cn

int size() const noexcept { return n_; }
来源：http://uph.jyoumei.cn

[S53] C++：移动语义
来源：http://xxj.yonumen.top

std::vector<int> w = std::move(v);
来源：http://ila.52xcode.cn

[S54] C++：异常处理
来源：http://fuq.zdqjudy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ncj.sjlbkw.cn

[S55] C++：结构化绑定
来源：http://zwr.vehdjk.com

auto [a, b] = std::make_pair(1, 2);
来源：http://ezp.hcnkem.com

[S56] C++：optional
来源：http://bqf.xuetiantiany.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ihr.dashuyun.cn

[S57] C++：编译期常量
来源：http://wie.zhaomingkeji.xyz

constexpr int N = 10;
来源：http://pxc.chenzaomai.com

[S58] C++：命名空间
来源：http://nhv.yanxiufei.cn

namespace ns { int f() { return 1; } }
来源：http://lfr.hammf.cn

[S59] C++：静态断言
来源：http://dmn.sxryk.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mul.yfazqb.com

[S60] C++：遍历并删除元素
来源：http://stm.feifeiyinyue.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ieb.shanyushiyangkeji.top

================================================================================
来源：http://xry.haohaochexian.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kle.bjfxy.top

================================================================================
来源：http://sok.xylfe.cn

[T01] Kotlin：Hello World
来源：http://pji.kuanghao11.cn

println("Hello")
来源：http://mgz.cucudq.cn

[T02] Kotlin：变量
来源：http://vid.snrcjt.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uwe.cashguo.top

[T03] Kotlin：字符串模板
来源：http://zmt.epnwcf.com

"值: $b"
来源：http://ixd.ctjpmb.com

[T04] Kotlin：空安全
来源：http://hpq.bbcook.cn

val n: String? = null;  n?.length
来源：http://pkt.svipenyu.cn

[T05] Kotlin：when 表达式
来源：http://exm.jinqigufen.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jpj.shzxlz.cn

[T06] Kotlin：集合映射
来源：http://ukh.guannengcc.top

listOf(1, 2, 3).map { it * 2 }
来源：http://gfj.tanke756.top

[T07] Kotlin：集合过滤
来源：http://tzw.feifeiyinyue.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://cud.yj202588.top

[T08] Kotlin：数据类
来源：http://uuw.zhaomingkeji.xyz

data class User(val name: String, val age: Int)
来源：http://umt.zhoulong.xyz

[T09] Kotlin：扩展函数
来源：http://wbb.ybcxt.top

fun String.exclaim() = this + "!"
来源：http://vxi.chenlongwang.top

[T10] Kotlin：默认参数
来源：http://fvf.fengsongda.top

fun greet(name: String = "World") = "Hi $name"
来源：http://gkt.vehdjk.com

[T11] Kotlin：协程
来源：http://vvs.jqgufenzy.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://sfm.yvedp.cn

[T12] Kotlin：解构声明
来源：http://heq.jiagoushi.top

val (a, b) = Pair(1, 2)
来源：http://foa.gogol.net.cn

[T13] Kotlin：只读 Map
来源：http://mrm.wangdashe.top

val m = mapOf("a" to 1)
来源：http://pro.sysykeji.top

[T14] Kotlin：循环
来源：http://kxh.ybcxt.top

for (i in 1..10) println(i)
来源：http://kjv.cucudq.cn


<!-- 参考信息 -->