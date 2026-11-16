代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mbq.316326.xyz

[R08] 数值比较
来源：http://faq.sysykeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://gci.zhongyouzk.top

[R09] 字符串比较
来源：http://rkb.vqdsnc.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ppg.c1oappe.top

[R10] 正则匹配
来源：http://uhs.ywan-chungtsiang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bqz.yangfankeji.com

[R11] case 多分支
来源：http://kkj.9152youxi.cn

case "$1" in
来源：http://hko.hywenlv.cn

start) echo "启动" ;;
来源：http://sri.hesvh.cn

stop)  echo "停止" ;;
来源：http://gbj.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://sps.xuanzx.com

esac
来源：http://dde.hcnkem.com

[R12] for 遍历文件
来源：http://rtr.shangyingyoupin.top

for f in *.txt; do echo "$f"; done
来源：http://grf.shangyingyoupin.top

[R13] for 计数循环
来源：http://seg.dianchejie.cn

for i in {1..10}; do echo "$i"; done
来源：http://vpl.guannengcc.top

[R14] C 风格 for
来源：http://ooh.shuidangran.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jyq.fktsv.cn

[R15] while 逐行读文件
来源：http://cpw.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://cld.hesvh.cn

[R16] until 等待条件
来源：http://vwm.bbcook.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://chk.zhijiandao.cn

[R17] 数组定义与取值
来源：http://gfc.zhixingplan.top

arr=(a b c); echo "${arr[0]}"
来源：http://xpg.shuidangran.top

[R18] 遍历数组
来源：http://odq.gaohongyu789.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nof.fehbvm.com

[R19] 数组长度
来源：http://hcz.mhx1999.top

echo "${#arr[@]}"
来源：http://gfi.cheryme.top

[R20] 关联数组（字典）
来源：http://nxv.yueranfly.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bwb.yongpay.top

[R21] 字符串长度
来源：http://jhz.ydjk.org.cn

echo "${#s}"
来源：http://phw.cucudq.cn

[R22] 截取子串
来源：http://nrc.yongpay.top

echo "${s:0:5}"
来源：http://voi.shanyushiyangtech.top

[R23] 字符串替换
来源：http://fky.fehbvm.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://isn.shuidangran.top

[R24] 大小写转换
来源：http://ill.havefunace.top

echo "${s^^}"; echo "${s,,}"
来源：http://nck.cucudq.cn

[R25] 去后缀 / 去前缀
来源：http://lam.andypj.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://rkc.jinqigufen.top

[R26] 命令替换
来源：http://bcm.quarkkingdee.top

now=$(date +%F); echo "$now"
来源：http://rsj.chenlongwang.top

[R27] 算术展开
来源：http://itk.jinyuanbaomall.cn

echo $((1 + 2 * 3))
来源：http://pmn.yfazqb.com

[R28] 浮点运算
来源：http://qlw.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://hve.nanxinkj.top

[R29] 定义函数
来源：http://lgq.zdqjudy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qqc.fzhhl.top

[R30] 函数返回状态码
来源：http://mhq.pengpengdd.cyou

f() { return 0; }; f || echo "失败了"
来源：http://xuk.hywenlv.cn

[R31] 局部变量
来源：http://osg.sxryk.cn

f() { local x=1; echo "$x"; }
来源：http://zfj.zycfv.cn

[R32] 参数个数校验
来源：http://cxd.cheryme.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uqz.fengsongda.top

[R33] 捕获错误并提示行号
来源：http://gph.gotoacloud.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://scc.bjfxy.top

[R34] 退出时清理
来源：http://qpq.fehbvm.com

trap 'rm -f "$tmp"' EXIT
来源：http://jpq.cheryme.top

[R35] 后台执行并等待
来源：http://rbo.tanke756.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hvg.ppjwa.cn

[R36] 并发执行多个任务
来源：http://dal.redwolf501.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zzq.ybcxt.top

[R37] 把输出赋给变量
来源：http://bbu.sysykeji.top

files=$(ls -1)
来源：http://mll.hnqzz.top

[R38] 管道串联
来源：http://deo.gaohongyu789.top

cat a.txt | grep -i error | wc -l
来源：http://bfr.iojbl.cn

[R39] 重定向标准输出与错误
来源：http://dcb.jiagoushi.top

cmd > out.log 2>&1
来源：http://fjf.shangyingyoupin.top

[R40] 追加写日志
来源：http://weh.jinqigufen.top

echo "log" >> out.log
来源：http://nah.xziqi.cn

[R41] 丢弃输出
来源：http://phq.nanxuanxn.top

cmd >/dev/null 2>&1
来源：http://wuk.hcnkem.com

[R42] 输入重定向
来源：http://ufv.jlsjyb.cn

wc -l < a.txt
来源：http://yao.fanxiaobao.xyz

[R43] 按名字查找文件
来源：http://ylj.zhijiandao.cn

find . -name "*.log" -type f
来源：http://bat.aizwys.cn

[R44] 按修改时间查找
来源：http://xlc.fzhhl.top

find . -mtime -7 -type f
来源：http://gkh.xziqi.cn

[R45] 批量删除
来源：http://tyd.zhoulong.xyz

find . -name "*.tmp" -delete
来源：http://cie.quarkkingdee.top

[R46] 递归替换文件内容
来源：http://rlu.epnwcf.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mhq.bbcook.cn

[R47] sed 单行替换
来源：http://bfv.ivvv.top

sed -i 's/foo/bar/g' a.txt
来源：http://uvi.yvedp.cn

[R48] awk 取指定列
来源：http://fqb.9152youxi.cn

awk '{print $1, $3}' a.txt
来源：http://xdw.yuxming.cn

[R49] awk 带条件
来源：http://cil.xylfe.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jpw.ydjk.org.cn

[R50] awk 求和
来源：http://zrr.vqdsnc.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lmd.ehwqpu.com

[R51] 排序去重取前几
来源：http://dfy.zhoulong.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://fdo.ydzc1.top

[R52] 统计行数
来源：http://tfc.shanyushiyangkeji.top

wc -l a.txt
来源：http://skc.zhengqikj.top

[R53] 查看文件头与实时尾
来源：http://upm.9152youxi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bay.yfazqb.com

[R54] 比较两个文件
来源：http://ats.quarkkingdee.top

diff a.txt b.txt
来源：http://hxs.wangdashe.top

[R55] 压缩与解压
来源：http://wfz.zhongyouzk.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ull.dashuyun.cn

[R56] 远程拷贝
来源：http://ztt.tanke756.top

scp file user@host:/path/
来源：http://zda.xziqi.cn

[R57] 远程执行命令
来源：http://lzz.xylfe.cn

ssh user@host 'uptime'
来源：http://vwo.yuanzhike.top

[R58] 下载文件
来源：http://xax.zdbjq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dcx.iojbl.cn

[R59] 发 POST JSON
来源：http://ukw.redwolf501.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dzj.0kj1m.cn

[R60] 只看 HTTP 状态码
来源：http://gwk.daria6918.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hbl.nwbrower.top

[R61] 磁盘占用
来源：http://ibd.shzxlz.cn

df -h;  du -sh *
来源：http://ypb.bbcook.cn

[R62] 找最占空间的文件
来源：http://zuf.kuanghao11.cn

du -ah . | sort -rh | head -10
来源：http://wtp.yj202588.top

[R63] 内存与进程
来源：http://ozu.jqgufenzy.top

free -h;  ps aux | grep nginx
来源：http://meh.nanxuanxn.top

[R64] 结束进程
来源：http://bxu.hongshengwenyu.top

kill -9 $(pgrep -f app.py)
来源：http://dfy.yj20258.top

[R65] 查看端口占用
来源：http://jdz.zhiwuduotai.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cqb.yj20258888.top

[R66] 定时任务
来源：http://nkp.chenlongwang.top

crontab -e;  crontab -l
来源：http://uud.xylfe.cn

[R67] 生成随机十六进制串
来源：http://rfy.aibaodan.cn

openssl rand -hex 16
来源：http://fmh.jqgfzy.top

[R68] 计算文件校验值
来源：http://isy.redwolf501.top

sha256sum a.txt;  md5sum a.txt
来源：http://web.dashuyun.cn

[R69] 生成随机密码
来源：http://vxn.cucudq.cn

head -c 16 /dev/urandom | base64
来源：http://uex.pycfn.com

[R70] 时间戳与互转
来源：http://lug.pycfn.com

date +%s;  date -d @1700000000
来源：http://rrz.sxryk.cn

[R71] 日期格式化
来源：http://qrj.yonumen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://fjx.bjfxy.top

[R72] 等待端口就绪
来源：http://ugc.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://iqm.guowangkeji.top

[R73] 分割大日志
来源：http://mqx.dianchejie.cn

split -l 1000 big.log part_
来源：http://dfi.shzxlz.cn

[R74] 批量重命名
来源：http://rck.yuxming.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nqm.gaohongyu789.top

[R75] 导出环境变量
来源：http://jbl.ywan-chungtsiang.top

export PATH="$HOME/bin:$PATH"
来源：http://neo.c1oappe.top

[R76] 使用临时文件
来源：http://xbg.hnxiangtu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lsj.316326.xyz

[R77] 读取用户输入
来源：http://plc.cqqwz.cn

read -rp "请输入: " ans
来源：http://eoo.jqgufenzy.top

[R78] 交互式菜单
来源：http://vts.zhijiandao.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ycg.zhijiandao.cn

[R79] 解析命令行选项
来源：http://fok.gaohongyu789.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mkq.zhaomingkeji.xyz

[R80] 查看脚本执行耗时
来源：http://ing.fktsv.cn

time ./run.sh
来源：http://qld.fanxiaobao.xyz

================================================================================
来源：http://kng.wangdashe.top

S. C / C++ 专题
来源：http://vve.epnwcf.com

================================================================================
来源：http://fcp.cqqwz.cn

[S01] C：Hello World
来源：http://yws.gzhubu.top

#include <stdio.h>
来源：http://auf.jqgufenzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vrz.jqgufenzy.top

[S02] C：变量与格式化输出
来源：http://beo.nwbrower.top

int a = 10; printf("%d\n", a);
来源：http://nys.tianlin.xyz

[S03] C：读入整数
来源：http://wjo.guowangkeji.top

int x; scanf("%d", &x);
来源：http://kka.yj202588.top

[S04] C：字符串复制
来源：http://uvr.daria6918.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mmp.jinqigfzy.top

[S05] C：字符串长度
来源：http://cgh.52xcode.cn

strlen(s)
来源：http://sef.hysaishi.cn

[S06] C：字符串比较
来源：http://oiw.mhx1999.top

strcmp(a, b) == 0
来源：http://asn.zdbjq.cn

[S07] C：数组遍历求和
来源：http://qqm.tianlin.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://iqa.iojbl.cn

[S08] C：动态内存分配与释放
来源：http://qll.zhijiandao.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xvy.zhijiandao.cn

[S09] C：结构体定义与初始化
来源：http://aly.ctjpmb.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tnq.sweek.top

[S10] C：指针与解引用
来源：http://spa.fktsv.cn

int *p = &a;  *p = 5;
来源：http://avc.cashguo.top

[S11] C：逐行读文件
来源：http://ukj.cdnleiting.top

FILE *f = fopen("a.txt", "r");
来源：http://nsg.hnxiangtu.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hxh.yanxiufei.cn

fclose(f);
来源：http://zkc.iojbl.cn

[S12] C：写文件
来源：http://sxz.ppjwa.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rhg.yonumen.top

[S13] C：宏定义
来源：http://hos.sysykeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vio.ydzc1.top

[S14] C：枚举
来源：http://sfc.cqqwz.cn

enum Color { RED, GREEN, BLUE };
来源：http://ihs.chenzaomai.com

[S15] C：类型转换
来源：http://uel.sjlbkw.cn

(double) a / b
来源：http://mdf.zhengqikj.top

[S16] C：位操作置位
来源：http://zcl.hnxiangtu.top

x |= (1 << 3);
来源：http://fkh.xingfuxueyuan.xyz

[S17] C：安全拼接字符串
来源：http://tje.sufxvd.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ita.fehbvm.com

[S18] C：命令行参数
来源：http://lot.52xcode.cn

int main(int argc, char **argv)
来源：http://ugc.cdnleiting.top

[S19] C：快速排序
来源：http://sxt.shuidangran.top

qsort(a, n, sizeof(int), cmp);
来源：http://jai.fanxiaobao.xyz

[S20] C：二分查找
来源：http://gpm.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wut.fehbvm.com

[S21] C：字符类别判断
来源：http://lpw.fanxiaobao.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cgc.xuanzx.com

[S22] C：字符串转数字
来源：http://kgr.hcnkem.com

atoi("42");  strtod("3.14", NULL);
来源：http://lgn.hnxiangtu.top

[S23] C：随机数
来源：http://tvl.pengpengdd.cyou

srand(time(NULL));  int r = rand() % 100;
来源：http://qnt.xuanzx.com

[S24] C：获取本地时间
来源：http://oqd.yanxiufei.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ujb.yj20258888.top

[S25] C：内存拷贝
来源：http://oya.zhongyouzk.top

memcpy(dst, src, n);
来源：http://cun.zhoulong.xyz

[S26] C：内存清零
来源：http://cja.nanxinkj.top

memset(a, 0, sizeof a);
来源：http://hxt.gzhubu.top

[S27] C：定义常量
来源：http://vuy.cheryme.top

const double PI = 3.14159;
来源：http://vtp.chenjidiqi.icu

[S28] C：静态变量
来源：http://wsk.kuanghao11.cn

static int counter = 0;
来源：http://reh.iojbl.cn

[S29] C：变参函数
来源：http://dyd.tian-w.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kve.fzhhl.top

[S30] C：头文件保护
来源：http://fng.sysykeji.top

#ifndef X_H
来源：http://wzv.ydjk.org.cn

#define X_H
来源：http://pbp.xinyue.icu

#endif
来源：http://prs.yonumen.top

[S31] C++：Hello World
来源：http://gjf.fehbvm.com

#include <iostream>
来源：http://tyl.sysykeji.top

int main() { std::cout << "Hello\n"; }
来源：http://uom.nanxinkj.top

[S32] C++：字符串
来源：http://kli.jinqigufen.top

std::string s = "hi";  s += "!";
来源：http://onc.birdmap.top

[S33] C++：vector 增删
来源：http://ffg.gaohongyu789.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wga.yangfankeji.com

[S34] C++：遍历 vector
来源：http://uiv.tianlin.xyz

for (auto &x : v) { std::cout << x; }
来源：http://smj.shzxlz.cn

[S35] C++：map
来源：http://jnm.bbcook.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mqa.cucudq.cn

[S36] C++：unordered_map
来源：http://qqv.zycfv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dlf.yj20258.top

[S37] C++：set
来源：http://jas.zdbjq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jml.tarul.cn

[S38] C++：排序
来源：http://hzw.hnqzz.top

std::sort(v.begin(), v.end());
来源：http://sgn.ivvv.top

[S39] C++：自定义比较器排序
来源：http://xik.jinyuanbaomall.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tof.hfpthk.cn

[S40] C++：查找元素
来源：http://res.shuidangran.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://njt.vehdjk.com

[S41] C++：类与构造函数
来源：http://lir.aibaodan.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cvy.jianghu66.top

[S42] C++：继承与虚函数
来源：http://tia.sjlbkw.cn

class B : public Base { public: void f() override {} };
来源：http://ecj.yj202588.top

[S43] C++：智能指针
来源：http://ter.shangyingyoupin.top

auto p = std::make_unique<int>(5);
来源：http://syu.zhongyouzk.top

[S44] C++：引用传参
来源：http://fhg.tianlin.xyz

void inc(int &x) { ++x; }
来源：http://emi.gogol.net.cn

[S45] C++：lambda
来源：http://rty.yj20258888.top

auto add = [](int a, int b) { return a + b; };
来源：http://mhi.hongshengwenyu.top

[S46] C++：函数模板
来源：http://zvx.jianghu66.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://phu.tian-w.cn

[S47] C++：结构化绑定遍历
来源：http://iri.jinghuilouyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mdc.c1oappe.top

[S48] C++：逐行读文件
来源：http://enl.sxryk.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lei.hysaishi.cn

while (std::getline(in, line)) { }
来源：http://cmx.shanyushiyangtech.top

[S49] C++：写文件
来源：http://dgt.fzhhl.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dtv.guannengcc.top

[S50] C++：格式化数字
来源：http://azt.yanxiufei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vkb.guannengcc.top

[S51] C++：显式类型转换
来源：http://zuj.zdqjudy.top

static_cast<double>(a) / b
来源：http://hic.chenzaomai.com

[S52] C++：const 与 noexcept
来源：http://yiq.wangdashe.top

int size() const noexcept { return n_; }
来源：http://bpq.xziqi.cn

[S53] C++：移动语义
来源：http://sxh.yangfankeji.com

std::vector<int> w = std::move(v);
来源：http://bjx.hesvh.cn

[S54] C++：异常处理
来源：http://tae.yfazqb.com

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mvt.cheryme.top

[S55] C++：结构化绑定
来源：http://svc.epnwcf.com

auto [a, b] = std::make_pair(1, 2);
来源：http://ifr.fengsongda.top

[S56] C++：optional
来源：http://dlv.0kj1m.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://flf.aizwys.cn

[S57] C++：编译期常量
来源：http://wdl.9152youxi.cn

constexpr int N = 10;
来源：http://vqx.fengsongda.top

[S58] C++：命名空间
来源：http://kwb.cashguo.top

namespace ns { int f() { return 1; } }
来源：http://szo.hcnkem.com

[S59] C++：静态断言
来源：http://idq.dianchejie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eya.xinyue.icu

[S60] C++：遍历并删除元素
来源：http://cfn.snrcjt.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://scb.yueranfly.top

================================================================================
来源：http://pvl.svipenyu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gex.cucudq.cn

================================================================================
来源：http://swf.meibo888.top

[T01] Kotlin：Hello World
来源：http://qlg.yj202588.top

println("Hello")
来源：http://tfy.feifeiyinyue.top

[T02] Kotlin：变量
来源：http://vmi.nwbrower.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yaf.mhx1999.top

[T03] Kotlin：字符串模板
来源：http://qzq.tian-w.cn

"值: $b"
来源：http://xlc.ybcxt.top

[T04] Kotlin：空安全
来源：http://jyx.pengpengdd.cyou

val n: String? = null;  n?.length
来源：http://fvv.jinyuanbaomall.cn

[T05] Kotlin：when 表达式
来源：http://lpz.xuetiantiany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qaj.xinyue.icu

[T06] Kotlin：集合映射
来源：http://onq.xuanzx.com

listOf(1, 2, 3).map { it * 2 }
来源：http://htp.birdmap.top

[T07] Kotlin：集合过滤
来源：http://vpt.ydjk.org.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://iwv.yangfankeji.com

[T08] Kotlin：数据类
来源：http://obf.hnxiangtu.top

data class User(val name: String, val age: Int)
来源：http://dvr.jinghuilouyu.cn


<!-- 参考信息 -->