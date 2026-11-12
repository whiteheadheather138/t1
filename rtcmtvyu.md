代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gnx.ivvv.top

[R08] 数值比较
来源：http://ppp.yuanzhike.top

if (( a > b )); then echo "a 更大"; fi
来源：http://bpo.zhixingplan.top

[R09] 字符串比较
来源：http://wxb.vehdjk.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kje.epnwcf.com

[R10] 正则匹配
来源：http://bwd.zhiwuduotai.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wsr.ctjpmb.com

[R11] case 多分支
来源：http://yew.gzhubu.top

case "$1" in
来源：http://hys.yonumen.top

start) echo "启动" ;;
来源：http://xuk.xuetiantiany.cn

stop)  echo "停止" ;;
来源：http://alq.hesvh.cn

*)     echo "未知命令" ;;
来源：http://ktn.zhaomingkeji.xyz

esac
来源：http://mgd.fengsongda.top

[R12] for 遍历文件
来源：http://gzu.tarul.cn

for f in *.txt; do echo "$f"; done
来源：http://cjn.hnxiangtu.top

[R13] for 计数循环
来源：http://ahq.sjlbkw.cn

for i in {1..10}; do echo "$i"; done
来源：http://ztr.tarul.cn

[R14] C 风格 for
来源：http://feg.ehwqpu.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xmx.daxiang520.top

[R15] while 逐行读文件
来源：http://vqq.sufxvd.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baa.smart0.xyz

[R16] until 等待条件
来源：http://hor.birdmap.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zig.fzhhl.top

[R17] 数组定义与取值
来源：http://ron.zycfv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vjs.meibo888.top

[R18] 遍历数组
来源：http://nnj.fanxiaobao.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://viw.shzxlz.cn

[R19] 数组长度
来源：http://ulw.vehdjk.com

echo "${#arr[@]}"
来源：http://fqh.52xcode.cn

[R20] 关联数组（字典）
来源：http://gug.shuidangran.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ozo.ctjpmb.com

[R21] 字符串长度
来源：http://css.fktsv.cn

echo "${#s}"
来源：http://rsq.dianchejie.cn

[R22] 截取子串
来源：http://zfi.shuidangran.top

echo "${s:0:5}"
来源：http://zzh.hysaishi.cn

[R23] 字符串替换
来源：http://oiq.zhijiandao.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ekv.smart0.xyz

[R24] 大小写转换
来源：http://fae.sysykeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://egu.dashuyun.cn

[R25] 去后缀 / 去前缀
来源：http://rms.cashguo.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://bnp.hammf.cn

[R26] 命令替换
来源：http://tjw.jqgfzy.top

now=$(date +%F); echo "$now"
来源：http://ldd.tian-w.cn

[R27] 算术展开
来源：http://sfs.nanxuanxn.top

echo $((1 + 2 * 3))
来源：http://fdi.xinyue.icu

[R28] 浮点运算
来源：http://ske.gotoacloud.top

echo "scale=2; 10/3" | bc
来源：http://xpy.jlsjyb.cn

[R29] 定义函数
来源：http://nsi.gogol.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jij.zhixingplan.top

[R30] 函数返回状态码
来源：http://izr.jianghu66.top

f() { return 0; }; f || echo "失败了"
来源：http://nbg.yj20258.top

[R31] 局部变量
来源：http://bvw.xylfe.cn

f() { local x=1; echo "$x"; }
来源：http://lmv.chenzaomai.com

[R32] 参数个数校验
来源：http://eki.pycfn.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zch.jyoumei.cn

[R33] 捕获错误并提示行号
来源：http://esl.vqdsnc.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bpo.gzhubu.top

[R34] 退出时清理
来源：http://fup.sweek.top

trap 'rm -f "$tmp"' EXIT
来源：http://vrn.ydjk.org.cn

[R35] 后台执行并等待
来源：http://khd.feifeiyinyue.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ajh.sufxvd.cn

[R36] 并发执行多个任务
来源：http://wqb.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lws.ybcxt.top

[R37] 把输出赋给变量
来源：http://hsn.bjfxy.top

files=$(ls -1)
来源：http://ael.sjlbkw.cn

[R38] 管道串联
来源：http://gbx.xylfe.cn

cat a.txt | grep -i error | wc -l
来源：http://gfq.fengsongda.top

[R39] 重定向标准输出与错误
来源：http://mwy.kuanghao11.cn

cmd > out.log 2>&1
来源：http://kjf.sweek.top

[R40] 追加写日志
来源：http://gzm.shanyushiyangkeji.top

echo "log" >> out.log
来源：http://ywn.dashuyun.cn

[R41] 丢弃输出
来源：http://dio.yvedp.cn

cmd >/dev/null 2>&1
来源：http://arh.pycfn.com

[R42] 输入重定向
来源：http://jko.gotoacloud.top

wc -l < a.txt
来源：http://pps.wangdashe.top

[R43] 按名字查找文件
来源：http://vbk.zdqjudy.top

find . -name "*.log" -type f
来源：http://pjl.tanke756.top

[R44] 按修改时间查找
来源：http://sbm.zdbjq.cn

find . -mtime -7 -type f
来源：http://uwi.ybcxt.top

[R45] 批量删除
来源：http://uxi.mhx1999.top

find . -name "*.tmp" -delete
来源：http://djv.yanxiufei.cn

[R46] 递归替换文件内容
来源：http://xio.tanke756.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sts.cashguo.top

[R47] sed 单行替换
来源：http://nhj.yanxiufei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://aum.shangyingyoupin.top

[R48] awk 取指定列
来源：http://mnt.xziqi.cn

awk '{print $1, $3}' a.txt
来源：http://zxk.jlsjyb.cn

[R49] awk 带条件
来源：http://lvq.zdqjudy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jmt.zdqjudy.top

[R50] awk 求和
来源：http://eap.yj20258888.top

awk '{s += $2} END {print s}' a.txt
来源：http://egx.hysaishi.cn

[R51] 排序去重取前几
来源：http://brn.jiagoushi.top

sort a.txt | uniq -c | sort -rn | head
来源：http://yaj.hywenlv.cn

[R52] 统计行数
来源：http://kly.havefunace.top

wc -l a.txt
来源：http://stz.tian-w.cn

[R53] 查看文件头与实时尾
来源：http://szq.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://agc.xylfe.cn

[R54] 比较两个文件
来源：http://jpx.cucudq.cn

diff a.txt b.txt
来源：http://umd.bbcook.cn

[R55] 压缩与解压
来源：http://ykw.dianchejie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hiy.tarul.cn

[R56] 远程拷贝
来源：http://lah.shuidangran.top

scp file user@host:/path/
来源：http://tqk.daxiang520.top

[R57] 远程执行命令
来源：http://vvb.tianlin.xyz

ssh user@host 'uptime'
来源：http://hdx.fengsongda.top

[R58] 下载文件
来源：http://tua.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://upl.aizwys.cn

[R59] 发 POST JSON
来源：http://zvc.daria6918.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mwq.wangdashe.top

[R60] 只看 HTTP 状态码
来源：http://usv.sysykeji.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hvn.ybcxt.top

[R61] 磁盘占用
来源：http://mgy.daria6918.cn

df -h;  du -sh *
来源：http://kww.kuanghao11.cn

[R62] 找最占空间的文件
来源：http://bqn.zdbjq.cn

du -ah . | sort -rh | head -10
来源：http://dos.yvedp.cn

[R63] 内存与进程
来源：http://lgh.ybcxt.top

free -h;  ps aux | grep nginx
来源：http://onw.aibaodan.cn

[R64] 结束进程
来源：http://klv.gotoacloud.top

kill -9 $(pgrep -f app.py)
来源：http://vxz.pengpengdd.cyou

[R65] 查看端口占用
来源：http://xik.nanxinkj.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zrd.yongpay.top

[R66] 定时任务
来源：http://bjd.cqqwz.cn

crontab -e;  crontab -l
来源：http://jtv.fengsongda.top

[R67] 生成随机十六进制串
来源：http://wvz.cdnleiting.top

openssl rand -hex 16
来源：http://crx.cqqwz.cn

[R68] 计算文件校验值
来源：http://zcv.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://skm.vqdsnc.cn

[R69] 生成随机密码
来源：http://ydj.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://fcs.hesvh.cn

[R70] 时间戳与互转
来源：http://dug.tarul.cn

date +%s;  date -d @1700000000
来源：http://gfe.hnqzz.top

[R71] 日期格式化
来源：http://khb.hammf.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hwk.xylfe.cn

[R72] 等待端口就绪
来源：http://rqn.tianlin.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://dmp.ydzc1.top

[R73] 分割大日志
来源：http://cos.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://ume.316326.xyz

[R74] 批量重命名
来源：http://uzj.cdnleiting.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wzp.c1oappe.top

[R75] 导出环境变量
来源：http://fib.hongshengwenyu.top

export PATH="$HOME/bin:$PATH"
来源：http://bot.wangdashe.top

[R76] 使用临时文件
来源：http://qgh.xylfe.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sxk.yongpay.top

[R77] 读取用户输入
来源：http://ppj.zhiwuduotai.top

read -rp "请输入: " ans
来源：http://vyt.jiagoushi.top

[R78] 交互式菜单
来源：http://ize.ehwqpu.com

select opt in a b c; do echo "$opt"; break; done
来源：http://wvq.pycfn.com

[R79] 解析命令行选项
来源：http://ubl.gzhubu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qtl.pycfn.com

[R80] 查看脚本执行耗时
来源：http://oyu.nanxuanxn.top

time ./run.sh
来源：http://cle.jinghuilouyu.cn

================================================================================
来源：http://rxl.jlsjyb.cn

S. C / C++ 专题
来源：http://fdl.fengsongda.top

================================================================================
来源：http://rqp.bbcook.cn

[S01] C：Hello World
来源：http://gha.kuanghao11.cn

#include <stdio.h>
来源：http://teb.ydjk.org.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jld.tanke756.top

[S02] C：变量与格式化输出
来源：http://rba.havefunace.top

int a = 10; printf("%d\n", a);
来源：http://gaq.zhengqikj.top

[S03] C：读入整数
来源：http://eep.gzhubu.top

int x; scanf("%d", &x);
来源：http://kfr.shanyushiyangtech.top

[S04] C：字符串复制
来源：http://frf.yueranfly.top

char dst[32]; strcpy(dst, "hi");
来源：http://gwy.daria6918.cn

[S05] C：字符串长度
来源：http://heh.shzxlz.cn

strlen(s)
来源：http://qpd.tarul.cn

[S06] C：字符串比较
来源：http://fff.chenlongwang.top

strcmp(a, b) == 0
来源：http://xvp.nanxuanxn.top

[S07] C：数组遍历求和
来源：http://pdu.nanxuanxn.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://owi.xingfuxueyuan.xyz

[S08] C：动态内存分配与释放
来源：http://xbb.ywan-chungtsiang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lmj.hammf.cn

[S09] C：结构体定义与初始化
来源：http://bxd.yanxiufei.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://szp.pengpengdd.cyou

[S10] C：指针与解引用
来源：http://cxr.nanxinkj.top

int *p = &a;  *p = 5;
来源：http://ctd.yj20258.top

[S11] C：逐行读文件
来源：http://vyh.ivvv.top

FILE *f = fopen("a.txt", "r");
来源：http://oxx.birdmap.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xtf.tarul.cn

fclose(f);
来源：http://rgy.9152youxi.cn

[S12] C：写文件
来源：http://mzx.hywenlv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yiz.xuanzx.com

[S13] C：宏定义
来源：http://ikk.sxryk.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ojk.tian-w.cn

[S14] C：枚举
来源：http://ppf.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://nkf.sjlbkw.cn

[S15] C：类型转换
来源：http://ioo.gotoacloud.top

(double) a / b
来源：http://ray.daxiang520.top

[S16] C：位操作置位
来源：http://qpq.xylfe.cn

x |= (1 << 3);
来源：http://ygd.zdbjq.cn

[S17] C：安全拼接字符串
来源：http://rwz.wangdashe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ijb.yj20258888.top

[S18] C：命令行参数
来源：http://gfr.vehdjk.com

int main(int argc, char **argv)
来源：http://ibh.ybcxt.top

[S19] C：快速排序
来源：http://gqg.bjfxy.top

qsort(a, n, sizeof(int), cmp);
来源：http://gft.guowangkeji.top

[S20] C：二分查找
来源：http://qky.yvedp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pmu.bjfxy.top

[S21] C：字符类别判断
来源：http://qhw.zdqjudy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ftx.havefunace.top

[S22] C：字符串转数字
来源：http://ttn.xinyue.icu

atoi("42");  strtod("3.14", NULL);
来源：http://axl.vehdjk.com

[S23] C：随机数
来源：http://ckf.snrcjt.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bgg.9152youxi.cn

[S24] C：获取本地时间
来源：http://pda.yonumen.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://out.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://omc.cdnleiting.top

memcpy(dst, src, n);
来源：http://jco.zhengqikj.top

[S26] C：内存清零
来源：http://bif.birdmap.top

memset(a, 0, sizeof a);
来源：http://fdk.yuxming.cn

[S27] C：定义常量
来源：http://tpi.fktsv.cn

const double PI = 3.14159;
来源：http://pwy.jyoumei.cn

[S28] C：静态变量
来源：http://vbq.hammf.cn

static int counter = 0;
来源：http://oma.shzxlz.cn

[S29] C：变参函数
来源：http://hcp.smart0.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vhv.sysykeji.top

[S30] C：头文件保护
来源：http://riv.zhaomingkeji.xyz

#ifndef X_H
来源：http://dcl.xziqi.cn

#define X_H
来源：http://yad.zhengqikj.top

#endif
来源：http://irh.haohaochexian.top

[S31] C++：Hello World
来源：http://sgi.smart0.xyz

#include <iostream>
来源：http://egm.zhoulong.xyz

int main() { std::cout << "Hello\n"; }
来源：http://ppb.yongpay.top

[S32] C++：字符串
来源：http://ivm.sysykeji.top

std::string s = "hi";  s += "!";
来源：http://rwj.yongpay.top

[S33] C++：vector 增删
来源：http://tet.iojbl.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kvd.smart0.xyz

[S34] C++：遍历 vector
来源：http://ilp.ywan-chungtsiang.top

for (auto &x : v) { std::cout << x; }
来源：http://vqw.gotoacloud.top

[S35] C++：map
来源：http://koq.gogol.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aei.yj202588.top

[S36] C++：unordered_map
来源：http://esj.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://lwe.cheryme.top

[S37] C++：set
来源：http://tuw.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uqe.ydzc1.top

[S38] C++：排序
来源：http://pav.316326.xyz

std::sort(v.begin(), v.end());
来源：http://uex.cashguo.top

[S39] C++：自定义比较器排序
来源：http://pgp.uphjek.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://afu.jqgufenzy.top

[S40] C++：查找元素
来源：http://sdj.xylfe.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://eqq.bbcook.cn

[S41] C++：类与构造函数
来源：http://hlv.9152youxi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://egm.yj202588.top

[S42] C++：继承与虚函数
来源：http://bof.tarul.cn

class B : public Base { public: void f() override {} };
来源：http://oew.snrcjt.cn

[S43] C++：智能指针
来源：http://ktr.yvedp.cn

auto p = std::make_unique<int>(5);
来源：http://naa.birdmap.top

[S44] C++：引用传参
来源：http://cqk.ivvv.top

void inc(int &x) { ++x; }
来源：http://yhu.daria6918.cn

[S45] C++：lambda
来源：http://kge.zhijiandao.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xkf.sxryk.cn

[S46] C++：函数模板
来源：http://hqc.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ttc.yuxming.cn

[S47] C++：结构化绑定遍历
来源：http://nli.gzhubu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kqi.zhiwuduotai.top

[S48] C++：逐行读文件
来源：http://uvp.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hqh.zhijiandao.cn

while (std::getline(in, line)) { }
来源：http://bke.316326.xyz

[S49] C++：写文件
来源：http://nqm.quarkkingdee.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ebg.nanxinkj.top

[S50] C++：格式化数字
来源：http://dwg.hfpthk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pux.xuetiantiany.cn

[S51] C++：显式类型转换
来源：http://sxu.shzxlz.cn

static_cast<double>(a) / b
来源：http://vdw.jinghuilouyu.cn

[S52] C++：const 与 noexcept
来源：http://zyj.zhixingplan.top

int size() const noexcept { return n_; }
来源：http://mgo.meibo888.top

[S53] C++：移动语义
来源：http://ukn.0kj1m.cn

std::vector<int> w = std::move(v);
来源：http://srw.smart0.xyz

[S54] C++：异常处理
来源：http://nol.jiagoushi.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gxn.ydjk.org.cn

[S55] C++：结构化绑定
来源：http://djd.uphjek.com

auto [a, b] = std::make_pair(1, 2);
来源：http://feg.hnqzz.top

[S56] C++：optional
来源：http://dsg.sjlbkw.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ifz.zhengqikj.top

[S57] C++：编译期常量
来源：http://quj.wangdashe.top

constexpr int N = 10;
来源：http://ila.epnwcf.com

[S58] C++：命名空间
来源：http://fsr.fanxiaobao.xyz

namespace ns { int f() { return 1; } }
来源：http://qpj.yfazqb.com

[S59] C++：静态断言
来源：http://cto.yj20258.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rfb.fzhhl.top

[S60] C++：遍历并删除元素
来源：http://bjm.ybcxt.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qle.daria6918.cn

================================================================================
来源：http://eye.jyoumei.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qsj.nanxinkj.top

================================================================================
来源：http://qun.hysaishi.cn

[T01] Kotlin：Hello World
来源：http://vha.bbcook.cn

println("Hello")
来源：http://wuz.kuanghao11.cn

[T02] Kotlin：变量
来源：http://yvr.hywenlv.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ftq.dianchejie.cn

[T03] Kotlin：字符串模板
来源：http://ste.hongshengwenyu.top

"值: $b"
来源：http://kbw.nanxinkj.top

[T04] Kotlin：空安全
来源：http://gdt.shuidangran.top

val n: String? = null;  n?.length
来源：http://zpg.shanyushiyangtech.top

[T05] Kotlin：when 表达式
来源：http://air.nanxuanxn.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wpz.aibaodan.cn

[T06] Kotlin：集合映射
来源：http://koo.bbcook.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://iwe.fktsv.cn

[T07] Kotlin：集合过滤
来源：http://iic.svipenyu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cwd.feifeiyinyue.top

[T08] Kotlin：数据类
来源：http://gxo.0kj1m.cn

data class User(val name: String, val age: Int)
来源：http://smw.wangdashe.top


<!-- 参考信息 -->