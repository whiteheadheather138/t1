代发 wailian999

esac
来源：http://ogx.yongpay.top

[R12] for 遍历文件
来源：http://lfw.yj20258888.top

for f in *.txt; do echo "$f"; done
来源：http://mpw.tianlin.xyz

[R13] for 计数循环
来源：http://duw.sxryk.cn

for i in {1..10}; do echo "$i"; done
来源：http://ojc.zycfv.cn

[R14] C 风格 for
来源：http://loz.cheryme.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ttv.shanyushiyangtech.top

[R15] while 逐行读文件
来源：http://qjm.hammf.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gkm.gotoacloud.top

[R16] until 等待条件
来源：http://tuf.jianghu66.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jpx.zycfv.cn

[R17] 数组定义与取值
来源：http://qvf.cdnleiting.top

arr=(a b c); echo "${arr[0]}"
来源：http://gna.shangyingyoupin.top

[R18] 遍历数组
来源：http://bka.xingfuxueyuan.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kah.hongshengwenyu.top

[R19] 数组长度
来源：http://kda.shzxlz.cn

echo "${#arr[@]}"
来源：http://gop.zhoulong.xyz

[R20] 关联数组（字典）
来源：http://sbj.zhengqikj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hah.ivvv.top

[R21] 字符串长度
来源：http://dix.daria6918.cn

echo "${#s}"
来源：http://vvu.nanxuanxn.top

[R22] 截取子串
来源：http://wrs.gogol.net.cn

echo "${s:0:5}"
来源：http://rne.nanxinkj.top

[R23] 字符串替换
来源：http://uqc.zdqjudy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pun.xylfe.cn

[R24] 大小写转换
来源：http://iua.xinyue.icu

echo "${s^^}"; echo "${s,,}"
来源：http://hzj.pycfn.com

[R25] 去后缀 / 去前缀
来源：http://mgj.ppjwa.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rtm.hammf.cn

[R26] 命令替换
来源：http://bbk.9152youxi.cn

now=$(date +%F); echo "$now"
来源：http://lnx.jlsjyb.cn

[R27] 算术展开
来源：http://ifq.shangyingyoupin.top

echo $((1 + 2 * 3))
来源：http://xzc.jinyuanbaomall.cn

[R28] 浮点运算
来源：http://oms.epnwcf.com

echo "scale=2; 10/3" | bc
来源：http://sch.hcnkem.com

[R29] 定义函数
来源：http://dbg.ppjwa.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://abg.jianghu66.top

[R30] 函数返回状态码
来源：http://vvq.andypj.xyz

f() { return 0; }; f || echo "失败了"
来源：http://voo.zhaomingkeji.xyz

[R31] 局部变量
来源：http://oed.hnxiangtu.top

f() { local x=1; echo "$x"; }
来源：http://wmd.hnxiangtu.top

[R32] 参数个数校验
来源：http://orn.jinqigfzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uye.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://iuk.sysykeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hxh.kuanghao11.cn

[R34] 退出时清理
来源：http://hdc.zhengqikj.top

trap 'rm -f "$tmp"' EXIT
来源：http://oab.cucudq.cn

[R35] 后台执行并等待
来源：http://egb.nanxuanxn.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vsb.wangshuangyany.cn

[R36] 并发执行多个任务
来源：http://pfg.fktsv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ghs.birdmap.top

[R37] 把输出赋给变量
来源：http://hoq.snrcjt.cn

files=$(ls -1)
来源：http://ffa.yj20258.top

[R38] 管道串联
来源：http://nea.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://vpt.nanxuanxn.top

[R39] 重定向标准输出与错误
来源：http://ahn.sjlbkw.cn

cmd > out.log 2>&1
来源：http://fqh.xziqi.cn

[R40] 追加写日志
来源：http://sqi.ivvv.top

echo "log" >> out.log
来源：http://jjb.bbcook.cn

[R41] 丢弃输出
来源：http://bin.gzhubu.top

cmd >/dev/null 2>&1
来源：http://yzc.shangyingyoupin.top

[R42] 输入重定向
来源：http://zkc.sysykeji.top

wc -l < a.txt
来源：http://xll.316326.xyz

[R43] 按名字查找文件
来源：http://vqt.fehbvm.com

find . -name "*.log" -type f
来源：http://tug.svipenyu.cn

[R44] 按修改时间查找
来源：http://pmy.zdbjq.cn

find . -mtime -7 -type f
来源：http://bjp.zhongyouzk.top

[R45] 批量删除
来源：http://olr.fktsv.cn

find . -name "*.tmp" -delete
来源：http://nku.yonumen.top

[R46] 递归替换文件内容
来源：http://tmb.feifeiyinyue.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qjt.jqgufenzy.top

[R47] sed 单行替换
来源：http://yxh.yj20258.top

sed -i 's/foo/bar/g' a.txt
来源：http://toy.cucudq.cn

[R48] awk 取指定列
来源：http://mja.cheryme.top

awk '{print $1, $3}' a.txt
来源：http://vcu.zhoulong.xyz

[R49] awk 带条件
来源：http://isj.sufxvd.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ctr.cashguo.top

[R50] awk 求和
来源：http://iwa.sysykeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://ids.cdnleiting.top

[R51] 排序去重取前几
来源：http://rnq.cdnleiting.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cse.xylfe.cn

[R52] 统计行数
来源：http://wdz.smart0.xyz

wc -l a.txt
来源：http://xza.ydjk.org.cn

[R53] 查看文件头与实时尾
来源：http://vtz.fanxiaobao.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ilv.tarul.cn

[R54] 比较两个文件
来源：http://giz.316326.xyz

diff a.txt b.txt
来源：http://fpl.sjlbkw.cn

[R55] 压缩与解压
来源：http://bsu.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wfa.nwbrower.top

[R56] 远程拷贝
来源：http://gpp.sweek.top

scp file user@host:/path/
来源：http://kkm.xylfe.cn

[R57] 远程执行命令
来源：http://fgc.quarkkingdee.top

ssh user@host 'uptime'
来源：http://ynk.hammf.cn

[R58] 下载文件
来源：http://ozu.sxryk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yux.pengpengdd.cyou

[R59] 发 POST JSON
来源：http://ief.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iai.hongshengwenyu.top

[R60] 只看 HTTP 状态码
来源：http://zwl.jyoumei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qeu.ppjwa.cn

[R61] 磁盘占用
来源：http://suj.fehbvm.com

df -h;  du -sh *
来源：http://qii.yj20258.top

[R62] 找最占空间的文件
来源：http://utf.hysaishi.cn

du -ah . | sort -rh | head -10
来源：http://dtw.meibo888.top

[R63] 内存与进程
来源：http://qsd.hnqzz.top

free -h;  ps aux | grep nginx
来源：http://vrz.ctjpmb.com

[R64] 结束进程
来源：http://fdk.xziqi.cn

kill -9 $(pgrep -f app.py)
来源：http://nvg.feifeiyinyue.top

[R65] 查看端口占用
来源：http://wfs.vehdjk.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zgz.zhiwuduotai.top

[R66] 定时任务
来源：http://qjw.hnxiangtu.top

crontab -e;  crontab -l
来源：http://yft.quarkkingdee.top

[R67] 生成随机十六进制串
来源：http://pgn.9152youxi.cn

openssl rand -hex 16
来源：http://tti.jlsjyb.cn

[R68] 计算文件校验值
来源：http://ahk.zhaomingkeji.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://ckt.yvedp.cn

[R69] 生成随机密码
来源：http://aom.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://fle.shuidangran.top

[R70] 时间戳与互转
来源：http://lft.cqqwz.cn

date +%s;  date -d @1700000000
来源：http://qvd.jinqigufen.top

[R71] 日期格式化
来源：http://nro.ywan-chungtsiang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kga.chenzaomai.com

[R72] 等待端口就绪
来源：http://xry.zhiwuduotai.top

until nc -z localhost 3306; do sleep 1; done
来源：http://beb.yueranfly.top

[R73] 分割大日志
来源：http://ubt.yanxiufei.cn

split -l 1000 big.log part_
来源：http://bsa.yongpay.top

[R74] 批量重命名
来源：http://vge.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hzc.quarkkingdee.top

[R75] 导出环境变量
来源：http://adf.redwolf501.top

export PATH="$HOME/bin:$PATH"
来源：http://had.cdnleiting.top

[R76] 使用临时文件
来源：http://rji.ehwqpu.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cvb.zhixingplan.top

[R77] 读取用户输入
来源：http://iwi.jyoumei.cn

read -rp "请输入: " ans
来源：http://mol.pycfn.com

[R78] 交互式菜单
来源：http://epr.jinqigufen.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fbi.zdbjq.cn

[R79] 解析命令行选项
来源：http://fod.jinqigfzy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://obv.jinghuilouyu.cn

[R80] 查看脚本执行耗时
来源：http://bca.hnqzz.top

time ./run.sh
来源：http://ncd.zhijiandao.cn

================================================================================
来源：http://lvu.guannengcc.top

S. C / C++ 专题
来源：http://heg.zdqjudy.top

================================================================================
来源：http://htf.9152youxi.cn

[S01] C：Hello World
来源：http://guv.52xcode.cn

#include <stdio.h>
来源：http://oud.nwbrower.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wuw.hnqzz.top

[S02] C：变量与格式化输出
来源：http://cmb.sxryk.cn

int a = 10; printf("%d\n", a);
来源：http://lfm.guannengcc.top

[S03] C：读入整数
来源：http://lff.feifeiyinyue.top

int x; scanf("%d", &x);
来源：http://rtc.redwolf501.top

[S04] C：字符串复制
来源：http://zpm.yongpay.top

char dst[32]; strcpy(dst, "hi");
来源：http://eju.chenzaomai.com

[S05] C：字符串长度
来源：http://kqa.zhoulong.xyz

strlen(s)
来源：http://nhf.gzhubu.top

[S06] C：字符串比较
来源：http://pkm.ydzc1.top

strcmp(a, b) == 0
来源：http://esw.zhaomingkeji.xyz

[S07] C：数组遍历求和
来源：http://prj.zycfv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dvm.zhiwuduotai.top

[S08] C：动态内存分配与释放
来源：http://gyu.hnxiangtu.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fhg.aizwys.cn

[S09] C：结构体定义与初始化
来源：http://eaf.0kj1m.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sia.wangshuangyany.cn

[S10] C：指针与解引用
来源：http://lkk.haohaochexian.top

int *p = &a;  *p = 5;
来源：http://ccn.gogol.net.cn

[S11] C：逐行读文件
来源：http://hik.xuanzx.com

FILE *f = fopen("a.txt", "r");
来源：http://kxl.daxiang520.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ggb.xuanzx.com

fclose(f);
来源：http://byw.yonumen.top

[S12] C：写文件
来源：http://ody.andypj.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://aiv.iojbl.cn

[S13] C：宏定义
来源：http://ogg.havefunace.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cdi.hammf.cn

[S14] C：枚举
来源：http://jxo.epnwcf.com

enum Color { RED, GREEN, BLUE };
来源：http://cyp.yonumen.top

[S15] C：类型转换
来源：http://uju.zhoulong.xyz

(double) a / b
来源：http://oea.sufxvd.cn

[S16] C：位操作置位
来源：http://fip.jiagoushi.top

x |= (1 << 3);
来源：http://lom.andypj.xyz

[S17] C：安全拼接字符串
来源：http://hry.sxryk.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kzm.mhx1999.top

[S18] C：命令行参数
来源：http://jdw.svipenyu.cn

int main(int argc, char **argv)
来源：http://amo.yonumen.top

[S19] C：快速排序
来源：http://cqv.shuidangran.top

qsort(a, n, sizeof(int), cmp);
来源：http://aja.ywan-chungtsiang.top

[S20] C：二分查找
来源：http://pdy.cheryme.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kpf.sxryk.cn

[S21] C：字符类别判断
来源：http://fch.chenlongwang.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cuv.snrcjt.cn

[S22] C：字符串转数字
来源：http://aig.jinyuanbaomall.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nyj.sjlbkw.cn

[S23] C：随机数
来源：http://ktd.ydzc1.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vid.316326.xyz

[S24] C：获取本地时间
来源：http://zlx.sxryk.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dvy.gotoacloud.top

[S25] C：内存拷贝
来源：http://bll.dianchejie.cn

memcpy(dst, src, n);
来源：http://msd.hcnkem.com

[S26] C：内存清零
来源：http://zlm.zhengqikj.top

memset(a, 0, sizeof a);
来源：http://twh.sxryk.cn

[S27] C：定义常量
来源：http://zrh.shanyushiyangkeji.top

const double PI = 3.14159;
来源：http://vfw.hfpthk.cn

[S28] C：静态变量
来源：http://sqv.hongshengwenyu.top

static int counter = 0;
来源：http://gxx.c1oappe.top

[S29] C：变参函数
来源：http://gsd.yueranfly.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aye.jyoumei.cn

[S30] C：头文件保护
来源：http://qun.ppjwa.cn

#ifndef X_H
来源：http://ivu.zhaomingkeji.xyz

#define X_H
来源：http://tto.zhiwuduotai.top

#endif
来源：http://gur.chenlongwang.top

[S31] C++：Hello World
来源：http://qqu.yangfankeji.com

#include <iostream>
来源：http://mqr.hywenlv.cn

int main() { std::cout << "Hello\n"; }
来源：http://kld.yonumen.top

[S32] C++：字符串
来源：http://lyr.fanxiaobao.xyz

std::string s = "hi";  s += "!";
来源：http://mng.316326.xyz

[S33] C++：vector 增删
来源：http://oby.feifeiyinyue.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nva.nwbrower.top

[S34] C++：遍历 vector
来源：http://drv.xuetiantiany.cn

for (auto &x : v) { std::cout << x; }
来源：http://can.nwbrower.top

[S35] C++：map
来源：http://big.zhoulong.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://eow.yueranfly.top

[S36] C++：unordered_map
来源：http://hid.aizwys.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iem.zhijiandao.cn

[S37] C++：set
来源：http://abj.yj202588.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lon.shangyingyoupin.top

[S38] C++：排序
来源：http://tun.yvedp.cn

std::sort(v.begin(), v.end());
来源：http://iap.ydjk.org.cn

[S39] C++：自定义比较器排序
来源：http://dgm.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ilg.zhengqikj.top

[S40] C++：查找元素
来源：http://fle.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iny.zhijiandao.cn

[S41] C++：类与构造函数
来源：http://dwd.yuanzhike.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qef.gogol.net.cn

[S42] C++：继承与虚函数
来源：http://kcc.iojbl.cn

class B : public Base { public: void f() override {} };
来源：http://cna.yueranfly.top

[S43] C++：智能指针
来源：http://tdl.nwbrower.top

auto p = std::make_unique<int>(5);
来源：http://zsw.bbcook.cn

[S44] C++：引用传参
来源：http://lrq.cucudq.cn

void inc(int &x) { ++x; }
来源：http://xxr.wangdashe.top

[S45] C++：lambda
来源：http://dyt.yanxiufei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wfd.ybcxt.top

[S46] C++：函数模板
来源：http://ykl.zycfv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://unz.c1oappe.top

[S47] C++：结构化绑定遍历
来源：http://tot.fzhhl.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lzn.snrcjt.cn

[S48] C++：逐行读文件
来源：http://iml.ydjk.org.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kmo.chenlongwang.top

while (std::getline(in, line)) { }
来源：http://huf.yvedp.cn

[S49] C++：写文件
来源：http://rzi.epnwcf.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mpt.shzxlz.cn

[S50] C++：格式化数字
来源：http://uri.hysaishi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hto.fanxiaobao.xyz

[S51] C++：显式类型转换
来源：http://gqt.zhoulong.xyz

static_cast<double>(a) / b
来源：http://hjk.gotoacloud.top

[S52] C++：const 与 noexcept
来源：http://dxb.yfazqb.com

int size() const noexcept { return n_; }
来源：http://vec.hywenlv.cn

[S53] C++：移动语义
来源：http://osc.cashguo.top

std::vector<int> w = std::move(v);
来源：http://zrk.sjlbkw.cn

[S54] C++：异常处理
来源：http://nrb.fzhhl.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cet.dianchejie.cn

[S55] C++：结构化绑定
来源：http://oxm.yj20258.top

auto [a, b] = std::make_pair(1, 2);
来源：http://fxv.jinqigfzy.top

[S56] C++：optional
来源：http://ckt.aibaodan.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xei.aizwys.cn

[S57] C++：编译期常量
来源：http://feh.sjlbkw.cn

constexpr int N = 10;
来源：http://hin.fzhhl.top

[S58] C++：命名空间
来源：http://snf.chenzaomai.com

namespace ns { int f() { return 1; } }
来源：http://zxq.fzhhl.top

[S59] C++：静态断言
来源：http://huf.zhongyouzk.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hfe.hammf.cn

[S60] C++：遍历并删除元素
来源：http://ros.nwbrower.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://iad.shangyingyoupin.top

================================================================================
来源：http://vcc.hfpthk.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xxp.gzhubu.top

================================================================================
来源：http://zna.9152youxi.cn

[T01] Kotlin：Hello World
来源：http://ipa.yj202588.top

println("Hello")
来源：http://hrb.shanyushiyangtech.top

[T02] Kotlin：变量
来源：http://ogt.shangyingyoupin.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wfq.shangyingyoupin.top

[T03] Kotlin：字符串模板
来源：http://dyi.pycfn.com

"值: $b"
来源：http://eqp.fzhhl.top

[T04] Kotlin：空安全
来源：http://ywp.hongshengwenyu.top

val n: String? = null;  n?.length
来源：http://ffz.pengpengdd.cyou

[T05] Kotlin：when 表达式
来源：http://hcv.yueranfly.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tvz.ywan-chungtsiang.top

[T06] Kotlin：集合映射
来源：http://bjr.xinyue.icu

listOf(1, 2, 3).map { it * 2 }
来源：http://mgo.jlsjyb.cn

[T07] Kotlin：集合过滤
来源：http://vue.zdqjudy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://bex.jqgufenzy.top

[T08] Kotlin：数据类
来源：http://omg.pengpengdd.cyou

data class User(val name: String, val age: Int)
来源：http://iqt.sxryk.cn

[T09] Kotlin：扩展函数
来源：http://fwb.shzxlz.cn

fun String.exclaim() = this + "!"
来源：http://vdn.jqgufenzy.top

[T10] Kotlin：默认参数
来源：http://bjo.jinghuilouyu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ntx.zhijiandao.cn

[T11] Kotlin：协程
来源：http://txi.jinqigufen.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://bud.sysykeji.top

[T12] Kotlin：解构声明
来源：http://nah.cucudq.cn

val (a, b) = Pair(1, 2)
来源：http://wfo.epnwcf.com

[T13] Kotlin：只读 Map
来源：http://kfu.ydjk.org.cn

val m = mapOf("a" to 1)
来源：http://jzy.gotoacloud.top

[T14] Kotlin：循环
来源：http://xzw.fengsongda.top

for (i in 1..10) println(i)
来源：http://izi.gaohongyu789.top


<!-- 参考信息 -->