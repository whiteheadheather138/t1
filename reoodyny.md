代发 wailian999

esac
来源：http://bji.cashguo.top

[R12] for 遍历文件
来源：http://ihd.cashguo.top

for f in *.txt; do echo "$f"; done
来源：http://voe.wangshuangyany.cn

[R13] for 计数循环
来源：http://beb.redwolf501.top

for i in {1..10}; do echo "$i"; done
来源：http://foq.hfpthk.cn

[R14] C 风格 for
来源：http://fbn.cdnleiting.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gju.kuanghao11.cn

[R15] while 逐行读文件
来源：http://otq.yuanzhike.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://etk.yanxiufei.cn

[R16] until 等待条件
来源：http://kfk.52xcode.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tjs.yueranfly.top

[R17] 数组定义与取值
来源：http://nis.xinyue.icu

arr=(a b c); echo "${arr[0]}"
来源：http://lge.yangfankeji.com

[R18] 遍历数组
来源：http://eay.yuxming.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://szu.ydjk.org.cn

[R19] 数组长度
来源：http://hly.jinyuanbaomall.cn

echo "${#arr[@]}"
来源：http://lsy.jiagoushi.top

[R20] 关联数组（字典）
来源：http://orz.kuanghao11.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ujp.feifeiyinyue.top

[R21] 字符串长度
来源：http://hqs.zycfv.cn

echo "${#s}"
来源：http://ucm.316326.xyz

[R22] 截取子串
来源：http://qmd.316326.xyz

echo "${s:0:5}"
来源：http://zdf.zhengqikj.top

[R23] 字符串替换
来源：http://bag.vehdjk.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ehp.jqgfzy.top

[R24] 大小写转换
来源：http://xsw.nwbrower.top

echo "${s^^}"; echo "${s,,}"
来源：http://idp.pengpengdd.cyou

[R25] 去后缀 / 去前缀
来源：http://cll.cucudq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ocy.epnwcf.com

[R26] 命令替换
来源：http://ioz.wangshuangyany.cn

now=$(date +%F); echo "$now"
来源：http://xzl.guowangkeji.top

[R27] 算术展开
来源：http://lxe.c1oappe.top

echo $((1 + 2 * 3))
来源：http://lhj.bjfxy.top

[R28] 浮点运算
来源：http://tjq.xylfe.cn

echo "scale=2; 10/3" | bc
来源：http://euh.daxiang520.top

[R29] 定义函数
来源：http://rjs.yanxiufei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://adz.316326.xyz

[R30] 函数返回状态码
来源：http://hla.aibaodan.cn

f() { return 0; }; f || echo "失败了"
来源：http://and.havefunace.top

[R31] 局部变量
来源：http://mar.birdmap.top

f() { local x=1; echo "$x"; }
来源：http://mul.shangyingyoupin.top

[R32] 参数个数校验
来源：http://qwv.haohaochexian.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rms.jinghuilouyu.cn

[R33] 捕获错误并提示行号
来源：http://yzn.xingfuxueyuan.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bsw.yongpay.top

[R34] 退出时清理
来源：http://iys.sysykeji.top

trap 'rm -f "$tmp"' EXIT
来源：http://cza.zdbjq.cn

[R35] 后台执行并等待
来源：http://vsm.jinqigufen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ejv.snrcjt.cn

[R36] 并发执行多个任务
来源：http://mof.zhijiandao.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oeb.fktsv.cn

[R37] 把输出赋给变量
来源：http://jtt.snrcjt.cn

files=$(ls -1)
来源：http://jxd.fktsv.cn

[R38] 管道串联
来源：http://jku.yj20258.top

cat a.txt | grep -i error | wc -l
来源：http://uro.wangshuangyany.cn

[R39] 重定向标准输出与错误
来源：http://jtv.havefunace.top

cmd > out.log 2>&1
来源：http://xjt.tanke756.top

[R40] 追加写日志
来源：http://ikj.vqdsnc.cn

echo "log" >> out.log
来源：http://ekc.meibo888.top

[R41] 丢弃输出
来源：http://age.yangfankeji.com

cmd >/dev/null 2>&1
来源：http://usf.yangfankeji.com

[R42] 输入重定向
来源：http://ktr.dianchejie.cn

wc -l < a.txt
来源：http://bsk.tarul.cn

[R43] 按名字查找文件
来源：http://pqz.yfazqb.com

find . -name "*.log" -type f
来源：http://dkg.zdbjq.cn

[R44] 按修改时间查找
来源：http://dxp.vehdjk.com

find . -mtime -7 -type f
来源：http://kvf.epnwcf.com

[R45] 批量删除
来源：http://ljq.hammf.cn

find . -name "*.tmp" -delete
来源：http://sns.daxiang520.top

[R46] 递归替换文件内容
来源：http://tlr.sufxvd.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cpl.zdbjq.cn

[R47] sed 单行替换
来源：http://clb.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://frz.guannengcc.top

[R48] awk 取指定列
来源：http://yuz.sjlbkw.cn

awk '{print $1, $3}' a.txt
来源：http://lzj.meibo888.top

[R49] awk 带条件
来源：http://evg.hywenlv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jfo.sjlbkw.cn

[R50] awk 求和
来源：http://hdn.cheryme.top

awk '{s += $2} END {print s}' a.txt
来源：http://cps.aizwys.cn

[R51] 排序去重取前几
来源：http://ypz.zycfv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ugi.fengsongda.top

[R52] 统计行数
来源：http://beu.jqgufenzy.top

wc -l a.txt
来源：http://sgg.daria6918.cn

[R53] 查看文件头与实时尾
来源：http://ajy.iojbl.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xlk.cheryme.top

[R54] 比较两个文件
来源：http://vgq.aizwys.cn

diff a.txt b.txt
来源：http://yqv.ctjpmb.com

[R55] 压缩与解压
来源：http://gxu.dianchejie.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ttv.xinyue.icu

[R56] 远程拷贝
来源：http://irm.jqgufenzy.top

scp file user@host:/path/
来源：http://dmu.cashguo.top

[R57] 远程执行命令
来源：http://nkf.zdbjq.cn

ssh user@host 'uptime'
来源：http://gij.ybcxt.top

[R58] 下载文件
来源：http://gln.zhengqikj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yhx.52xcode.cn

[R59] 发 POST JSON
来源：http://hzm.ywan-chungtsiang.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cor.yangfankeji.com

[R60] 只看 HTTP 状态码
来源：http://yku.sufxvd.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qsi.svipenyu.cn

[R61] 磁盘占用
来源：http://thn.vqdsnc.cn

df -h;  du -sh *
来源：http://ptk.52xcode.cn

[R62] 找最占空间的文件
来源：http://dwb.tianlin.xyz

du -ah . | sort -rh | head -10
来源：http://pdh.xziqi.cn

[R63] 内存与进程
来源：http://osg.mhx1999.top

free -h;  ps aux | grep nginx
来源：http://uxh.tianlin.xyz

[R64] 结束进程
来源：http://coz.hcnkem.com

kill -9 $(pgrep -f app.py)
来源：http://hfs.jianghu66.top

[R65] 查看端口占用
来源：http://fbd.xziqi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wmf.ivvv.top

[R66] 定时任务
来源：http://elj.daxiang520.top

crontab -e;  crontab -l
来源：http://hjn.daxiang520.top

[R67] 生成随机十六进制串
来源：http://omk.zhiwuduotai.top

openssl rand -hex 16
来源：http://cce.fehbvm.com

[R68] 计算文件校验值
来源：http://ocg.cucudq.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jzi.gzhubu.top

[R69] 生成随机密码
来源：http://hoi.yj202588.top

head -c 16 /dev/urandom | base64
来源：http://slq.ywan-chungtsiang.top

[R70] 时间戳与互转
来源：http://wcq.wangdashe.top

date +%s;  date -d @1700000000
来源：http://ahu.cdnleiting.top

[R71] 日期格式化
来源：http://ffb.hysaishi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yno.smart0.xyz

[R72] 等待端口就绪
来源：http://oqs.haohaochexian.top

until nc -z localhost 3306; do sleep 1; done
来源：http://bfp.yueranfly.top

[R73] 分割大日志
来源：http://gtc.daxiang520.top

split -l 1000 big.log part_
来源：http://xzn.redwolf501.top

[R74] 批量重命名
来源：http://ota.gzhubu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rpe.haohaochexian.top

[R75] 导出环境变量
来源：http://lsg.ywan-chungtsiang.top

export PATH="$HOME/bin:$PATH"
来源：http://xpj.c1oappe.top

[R76] 使用临时文件
来源：http://eld.hysaishi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://her.redwolf501.top

[R77] 读取用户输入
来源：http://enk.hongshengwenyu.top

read -rp "请输入: " ans
来源：http://uim.shanyushiyangtech.top

[R78] 交互式菜单
来源：http://wsc.gogol.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nik.tian-w.cn

[R79] 解析命令行选项
来源：http://kse.jinyuanbaomall.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zco.zhengqikj.top

[R80] 查看脚本执行耗时
来源：http://apa.zhongyouzk.top

time ./run.sh
来源：http://fqj.vehdjk.com

================================================================================
来源：http://ihi.jinqigfzy.top

S. C / C++ 专题
来源：http://eln.nwbrower.top

================================================================================
来源：http://jmr.andypj.xyz

[S01] C：Hello World
来源：http://jjb.hongshengwenyu.top

#include <stdio.h>
来源：http://zix.guannengcc.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://gbb.bjfxy.top

[S02] C：变量与格式化输出
来源：http://cnd.andypj.xyz

int a = 10; printf("%d\n", a);
来源：http://uvo.daxiang520.top

[S03] C：读入整数
来源：http://vqh.jinqigfzy.top

int x; scanf("%d", &x);
来源：http://jcg.yfazqb.com

[S04] C：字符串复制
来源：http://vfx.316326.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://bee.jqgufenzy.top

[S05] C：字符串长度
来源：http://tgm.cheryme.top

strlen(s)
来源：http://nbk.feifeiyinyue.top

[S06] C：字符串比较
来源：http://vat.uphjek.com

strcmp(a, b) == 0
来源：http://ort.yonumen.top

[S07] C：数组遍历求和
来源：http://wzg.xylfe.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zas.zhijiandao.cn

[S08] C：动态内存分配与释放
来源：http://kev.cashguo.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hrm.ctjpmb.com

[S09] C：结构体定义与初始化
来源：http://oxt.wangdashe.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xnw.ybcxt.top

[S10] C：指针与解引用
来源：http://fum.ivvv.top

int *p = &a;  *p = 5;
来源：http://wlq.tianlin.xyz

[S11] C：逐行读文件
来源：http://gzr.fehbvm.com

FILE *f = fopen("a.txt", "r");
来源：http://jij.yvedp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://hdz.chenzaomai.com

fclose(f);
来源：http://zmr.shanyushiyangtech.top

[S12] C：写文件
来源：http://iwh.cashguo.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kfv.tarul.cn

[S13] C：宏定义
来源：http://lsa.fehbvm.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ugs.ehwqpu.com

[S14] C：枚举
来源：http://xrc.guowangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://iwo.shangyingyoupin.top

[S15] C：类型转换
来源：http://mch.xingfuxueyuan.xyz

(double) a / b
来源：http://wit.0kj1m.cn

[S16] C：位操作置位
来源：http://hlg.nanxuanxn.top

x |= (1 << 3);
来源：http://mrm.jqgfzy.top

[S17] C：安全拼接字符串
来源：http://van.hnqzz.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://smq.iojbl.cn

[S18] C：命令行参数
来源：http://tes.haohaochexian.top

int main(int argc, char **argv)
来源：http://xqz.ywan-chungtsiang.top

[S19] C：快速排序
来源：http://atw.smart0.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://ubn.tianlin.xyz

[S20] C：二分查找
来源：http://nop.yanxiufei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mok.jqgufenzy.top

[S21] C：字符类别判断
来源：http://okm.ppjwa.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rfc.hongshengwenyu.top

[S22] C：字符串转数字
来源：http://pfg.zdqjudy.top

atoi("42");  strtod("3.14", NULL);
来源：http://zxb.yangfankeji.com

[S23] C：随机数
来源：http://cfi.zdbjq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uvi.yonumen.top

[S24] C：获取本地时间
来源：http://jli.9152youxi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gqw.sysykeji.top

[S25] C：内存拷贝
来源：http://kxa.hnxiangtu.top

memcpy(dst, src, n);
来源：http://fvc.hongshengwenyu.top

[S26] C：内存清零
来源：http://wrg.yuxming.cn

memset(a, 0, sizeof a);
来源：http://xnz.uphjek.com

[S27] C：定义常量
来源：http://kiv.vqdsnc.cn

const double PI = 3.14159;
来源：http://oac.jinyuanbaomall.cn

[S28] C：静态变量
来源：http://tfe.c1oappe.top

static int counter = 0;
来源：http://ump.hammf.cn

[S29] C：变参函数
来源：http://iiv.52xcode.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tgq.bjfxy.top

[S30] C：头文件保护
来源：http://krq.fengsongda.top

#ifndef X_H
来源：http://aiv.xuanzx.com

#define X_H
来源：http://bat.iojbl.cn

#endif
来源：http://fli.yj20258.top

[S31] C++：Hello World
来源：http://ikj.ctjpmb.com

#include <iostream>
来源：http://ckp.hysaishi.cn

int main() { std::cout << "Hello\n"; }
来源：http://aey.hysaishi.cn

[S32] C++：字符串
来源：http://usv.zhoulong.xyz

std::string s = "hi";  s += "!";
来源：http://qpp.hywenlv.cn

[S33] C++：vector 增删
来源：http://aej.dashuyun.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ivu.yfazqb.com

[S34] C++：遍历 vector
来源：http://rmj.zycfv.cn

for (auto &x : v) { std::cout << x; }
来源：http://ndv.ehwqpu.com

[S35] C++：map
来源：http://rxo.yvedp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pky.jlsjyb.cn

[S36] C++：unordered_map
来源：http://rpr.wangshuangyany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gcd.0kj1m.cn

[S37] C++：set
来源：http://bba.zdbjq.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zzd.daria6918.cn

[S38] C++：排序
来源：http://ufo.zdqjudy.top

std::sort(v.begin(), v.end());
来源：http://xxv.daria6918.cn

[S39] C++：自定义比较器排序
来源：http://vxy.pengpengdd.cyou

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jea.yvedp.cn

[S40] C++：查找元素
来源：http://qip.birdmap.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://law.c1oappe.top

[S41] C++：类与构造函数
来源：http://jnd.chenzaomai.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nre.dianchejie.cn

[S42] C++：继承与虚函数
来源：http://zpc.ydjk.org.cn

class B : public Base { public: void f() override {} };
来源：http://bmm.ctjpmb.com

[S43] C++：智能指针
来源：http://evr.sysykeji.top

auto p = std::make_unique<int>(5);
来源：http://bps.yongpay.top

[S44] C++：引用传参
来源：http://odh.quarkkingdee.top

void inc(int &x) { ++x; }
来源：http://cma.mhx1999.top

[S45] C++：lambda
来源：http://kpq.dashuyun.cn

auto add = [](int a, int b) { return a + b; };
来源：http://avj.cashguo.top

[S46] C++：函数模板
来源：http://xpp.cucudq.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wtl.zhiwuduotai.top

[S47] C++：结构化绑定遍历
来源：http://yqv.zhengqikj.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gna.jiagoushi.top

[S48] C++：逐行读文件
来源：http://gvn.hysaishi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fcv.c1oappe.top

while (std::getline(in, line)) { }
来源：http://iqx.sjlbkw.cn

[S49] C++：写文件
来源：http://rlx.chenlongwang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kcg.nwbrower.top

[S50] C++：格式化数字
来源：http://jsd.vqdsnc.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://djl.shangyingyoupin.top

[S51] C++：显式类型转换
来源：http://jpx.yueranfly.top

static_cast<double>(a) / b
来源：http://odk.jianghu66.top

[S52] C++：const 与 noexcept
来源：http://gec.jinqigfzy.top

int size() const noexcept { return n_; }
来源：http://zir.zdbjq.cn

[S53] C++：移动语义
来源：http://fpp.cqqwz.cn

std::vector<int> w = std::move(v);
来源：http://juc.svipenyu.cn

[S54] C++：异常处理
来源：http://stj.guannengcc.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pok.gogol.net.cn

[S55] C++：结构化绑定
来源：http://tqr.hesvh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://oqp.fanxiaobao.xyz

[S56] C++：optional
来源：http://hws.epnwcf.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qvy.ehwqpu.com

[S57] C++：编译期常量
来源：http://wzi.snrcjt.cn

constexpr int N = 10;
来源：http://ovj.haohaochexian.top

[S58] C++：命名空间
来源：http://gyj.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://xbm.svipenyu.cn

[S59] C++：静态断言
来源：http://nua.zhaomingkeji.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gan.vqdsnc.cn

[S60] C++：遍历并删除元素
来源：http://zsg.jiagoushi.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wzk.jinghuilouyu.cn

================================================================================
来源：http://nvm.daxiang520.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vex.uphjek.com

================================================================================
来源：http://ktq.cheryme.top

[T01] Kotlin：Hello World
来源：http://lgs.fanxiaobao.xyz

println("Hello")
来源：http://oxt.zdbjq.cn

[T02] Kotlin：变量
来源：http://kjf.cdnleiting.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uum.birdmap.top

[T03] Kotlin：字符串模板
来源：http://tki.hysaishi.cn

"值: $b"
来源：http://diu.zdqjudy.top

[T04] Kotlin：空安全
来源：http://dst.gzhubu.top

val n: String? = null;  n?.length
来源：http://uih.nanxuanxn.top

[T05] Kotlin：when 表达式
来源：http://kii.yuxming.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://awa.ywan-chungtsiang.top

[T06] Kotlin：集合映射
来源：http://mej.zhaomingkeji.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://asc.hysaishi.cn

[T07] Kotlin：集合过滤
来源：http://qee.ivvv.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://jkq.pengpengdd.cyou

[T08] Kotlin：数据类
来源：http://ybc.jiagoushi.top

data class User(val name: String, val age: Int)
来源：http://yxi.yvedp.cn

[T09] Kotlin：扩展函数
来源：http://yfm.svipenyu.cn

fun String.exclaim() = this + "!"
来源：http://pis.0kj1m.cn

[T10] Kotlin：默认参数
来源：http://ykm.zhijiandao.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ofq.gaohongyu789.top

[T11] Kotlin：协程
来源：http://akh.hongshengwenyu.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://wvl.yanxiufei.cn

[T12] Kotlin：解构声明
来源：http://puq.uphjek.com

val (a, b) = Pair(1, 2)
来源：http://uou.fengsongda.top

[T13] Kotlin：只读 Map
来源：http://rhz.jinqigufen.top

val m = mapOf("a" to 1)
来源：http://ltt.9152youxi.cn

[T14] Kotlin：循环
来源：http://cgt.epnwcf.com

for (i in 1..10) println(i)
来源：http://keq.gaohongyu789.top


<!-- 参考信息 -->