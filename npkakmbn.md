代发 wailian999

echo "${#arr[@]}"
来源：http://whw.hesvh.cn

[R20] 关联数组（字典）
来源：http://dac.zhengqikj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uej.shanyushiyangtech.top

[R21] 字符串长度
来源：http://ypq.quarkkingdee.top

echo "${#s}"
来源：http://brb.jinyuanbaomall.cn

[R22] 截取子串
来源：http://jjn.fengsongda.top

echo "${s:0:5}"
来源：http://deg.gzhubu.top

[R23] 字符串替换
来源：http://bne.52xcode.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dxu.tanke756.top

[R24] 大小写转换
来源：http://gdt.shzxlz.cn

echo "${s^^}"; echo "${s,,}"
来源：http://fez.ppjwa.cn

[R25] 去后缀 / 去前缀
来源：http://zvs.snrcjt.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nnm.bjfxy.top

[R26] 命令替换
来源：http://ffg.yongpay.top

now=$(date +%F); echo "$now"
来源：http://yvi.dashuyun.cn

[R27] 算术展开
来源：http://ezd.yueranfly.top

echo $((1 + 2 * 3))
来源：http://vnn.jlsjyb.cn

[R28] 浮点运算
来源：http://dvn.shangyingyoupin.top

echo "scale=2; 10/3" | bc
来源：http://hjx.mhx1999.top

[R29] 定义函数
来源：http://dxu.daxiang520.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uoe.yanxiufei.cn

[R30] 函数返回状态码
来源：http://qkl.0kj1m.cn

f() { return 0; }; f || echo "失败了"
来源：http://nco.nanxuanxn.top

[R31] 局部变量
来源：http://lpn.tarul.cn

f() { local x=1; echo "$x"; }
来源：http://cra.jinyuanbaomall.cn

[R32] 参数个数校验
来源：http://dwd.xingfuxueyuan.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://imb.wangshuangyany.cn

[R33] 捕获错误并提示行号
来源：http://vzc.yonumen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rdv.xziqi.cn

[R34] 退出时清理
来源：http://eba.hywenlv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ctn.ctjpmb.com

[R35] 后台执行并等待
来源：http://fvm.zhijiandao.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://kwp.jinghuilouyu.cn

[R36] 并发执行多个任务
来源：http://ijx.sweek.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gjf.yongpay.top

[R37] 把输出赋给变量
来源：http://nnl.bbcook.cn

files=$(ls -1)
来源：http://frw.cashguo.top

[R38] 管道串联
来源：http://ill.haohaochexian.top

cat a.txt | grep -i error | wc -l
来源：http://gdt.sxryk.cn

[R39] 重定向标准输出与错误
来源：http://wxp.yj20258.top

cmd > out.log 2>&1
来源：http://eah.quarkkingdee.top

[R40] 追加写日志
来源：http://mho.zhijiandao.cn

echo "log" >> out.log
来源：http://pfu.sxryk.cn

[R41] 丢弃输出
来源：http://bbb.yvedp.cn

cmd >/dev/null 2>&1
来源：http://hks.hnxiangtu.top

[R42] 输入重定向
来源：http://ocw.yj202588.top

wc -l < a.txt
来源：http://hvf.iojbl.cn

[R43] 按名字查找文件
来源：http://ith.mhx1999.top

find . -name "*.log" -type f
来源：http://fal.birdmap.top

[R44] 按修改时间查找
来源：http://abz.jinqigfzy.top

find . -mtime -7 -type f
来源：http://gym.yj20258.top

[R45] 批量删除
来源：http://nug.jlsjyb.cn

find . -name "*.tmp" -delete
来源：http://bww.wangshuangyany.cn

[R46] 递归替换文件内容
来源：http://ysf.haohaochexian.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rnu.daxiang520.top

[R47] sed 单行替换
来源：http://geg.yvedp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mpv.sjlbkw.cn

[R48] awk 取指定列
来源：http://uig.tanke756.top

awk '{print $1, $3}' a.txt
来源：http://qny.kuanghao11.cn

[R49] awk 带条件
来源：http://ptc.birdmap.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nap.pycfn.com

[R50] awk 求和
来源：http://oba.hnqzz.top

awk '{s += $2} END {print s}' a.txt
来源：http://bmv.gaohongyu789.top

[R51] 排序去重取前几
来源：http://nvd.xuetiantiany.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xqy.ehwqpu.com

[R52] 统计行数
来源：http://vfq.ydzc1.top

wc -l a.txt
来源：http://pff.sjlbkw.cn

[R53] 查看文件头与实时尾
来源：http://tsm.zdbjq.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kwf.feifeiyinyue.top

[R54] 比较两个文件
来源：http://lgz.smart0.xyz

diff a.txt b.txt
来源：http://kgs.ydjk.org.cn

[R55] 压缩与解压
来源：http://hig.yangfankeji.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kin.zdbjq.cn

[R56] 远程拷贝
来源：http://owm.smart0.xyz

scp file user@host:/path/
来源：http://qft.shanyushiyangkeji.top

[R57] 远程执行命令
来源：http://hxy.hesvh.cn

ssh user@host 'uptime'
来源：http://bkq.zdbjq.cn

[R58] 下载文件
来源：http://tks.birdmap.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kfy.meibo888.top

[R59] 发 POST JSON
来源：http://igc.gogol.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mcj.mhx1999.top

[R60] 只看 HTTP 状态码
来源：http://zji.9152youxi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://keu.smart0.xyz

[R61] 磁盘占用
来源：http://ezy.chenlongwang.top

df -h;  du -sh *
来源：http://lhh.gzhubu.top

[R62] 找最占空间的文件
来源：http://jtb.hysaishi.cn

du -ah . | sort -rh | head -10
来源：http://ysj.cashguo.top

[R63] 内存与进程
来源：http://ywa.yuanzhike.top

free -h;  ps aux | grep nginx
来源：http://ild.tarul.cn

[R64] 结束进程
来源：http://wws.nwbrower.top

kill -9 $(pgrep -f app.py)
来源：http://tdd.cucudq.cn

[R65] 查看端口占用
来源：http://wwc.cdnleiting.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dtn.cashguo.top

[R66] 定时任务
来源：http://amc.guannengcc.top

crontab -e;  crontab -l
来源：http://kgb.9152youxi.cn

[R67] 生成随机十六进制串
来源：http://iex.yueranfly.top

openssl rand -hex 16
来源：http://fcx.shanyushiyangkeji.top

[R68] 计算文件校验值
来源：http://whx.daria6918.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hkd.andypj.xyz

[R69] 生成随机密码
来源：http://hrc.havefunace.top

head -c 16 /dev/urandom | base64
来源：http://xqs.tianlin.xyz

[R70] 时间戳与互转
来源：http://bvs.haohaochexian.top

date +%s;  date -d @1700000000
来源：http://kdv.epnwcf.com

[R71] 日期格式化
来源：http://ulh.fanxiaobao.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://nal.sysykeji.top

[R72] 等待端口就绪
来源：http://mgy.sjlbkw.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://lhu.tianlin.xyz

[R73] 分割大日志
来源：http://han.xuetiantiany.cn

split -l 1000 big.log part_
来源：http://yos.jiagoushi.top

[R74] 批量重命名
来源：http://lmb.tianlin.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sec.yj20258888.top

[R75] 导出环境变量
来源：http://vbb.ybcxt.top

export PATH="$HOME/bin:$PATH"
来源：http://lyi.gaohongyu789.top

[R76] 使用临时文件
来源：http://nrt.cheryme.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://osl.chenlongwang.top

[R77] 读取用户输入
来源：http://wzq.vehdjk.com

read -rp "请输入: " ans
来源：http://roq.jqgufenzy.top

[R78] 交互式菜单
来源：http://mlv.yongpay.top

select opt in a b c; do echo "$opt"; break; done
来源：http://npl.zhiwuduotai.top

[R79] 解析命令行选项
来源：http://xis.meibo888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zmq.yuanzhike.top

[R80] 查看脚本执行耗时
来源：http://gxe.fktsv.cn

time ./run.sh
来源：http://qtm.xinyue.icu

================================================================================
来源：http://wpo.haohaochexian.top

S. C / C++ 专题
来源：http://pyy.haohaochexian.top

================================================================================
来源：http://xid.dashuyun.cn

[S01] C：Hello World
来源：http://exc.meibo888.top

#include <stdio.h>
来源：http://gmb.dashuyun.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rfk.pycfn.com

[S02] C：变量与格式化输出
来源：http://yhe.cqqwz.cn

int a = 10; printf("%d\n", a);
来源：http://syj.kuanghao11.cn

[S03] C：读入整数
来源：http://pli.shanyushiyangtech.top

int x; scanf("%d", &x);
来源：http://lib.wangshuangyany.cn

[S04] C：字符串复制
来源：http://oxh.yuxming.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rwk.0kj1m.cn

[S05] C：字符串长度
来源：http://olp.cqqwz.cn

strlen(s)
来源：http://ubn.fengsongda.top

[S06] C：字符串比较
来源：http://cms.zhixingplan.top

strcmp(a, b) == 0
来源：http://fju.c1oappe.top

[S07] C：数组遍历求和
来源：http://mzl.daria6918.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dvw.yuanzhike.top

[S08] C：动态内存分配与释放
来源：http://uof.hysaishi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pvz.hywenlv.cn

[S09] C：结构体定义与初始化
来源：http://vsg.havefunace.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lav.smart0.xyz

[S10] C：指针与解引用
来源：http://fha.jinqigfzy.top

int *p = &a;  *p = 5;
来源：http://vdv.ehwqpu.com

[S11] C：逐行读文件
来源：http://xgw.chenzaomai.com

FILE *f = fopen("a.txt", "r");
来源：http://edo.cdnleiting.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://oyd.tian-w.cn

fclose(f);
来源：http://efi.fzhhl.top

[S12] C：写文件
来源：http://sks.uphjek.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fbu.jqgfzy.top

[S13] C：宏定义
来源：http://afs.yongpay.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ntj.hesvh.cn

[S14] C：枚举
来源：http://mkj.dianchejie.cn

enum Color { RED, GREEN, BLUE };
来源：http://sdi.yj20258.top

[S15] C：类型转换
来源：http://ojd.jinyuanbaomall.cn

(double) a / b
来源：http://fuk.chenlongwang.top

[S16] C：位操作置位
来源：http://hcn.shanyushiyangkeji.top

x |= (1 << 3);
来源：http://krg.dashuyun.cn

[S17] C：安全拼接字符串
来源：http://duo.hnqzz.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cym.316326.xyz

[S18] C：命令行参数
来源：http://cxw.zdqjudy.top

int main(int argc, char **argv)
来源：http://dlw.epnwcf.com

[S19] C：快速排序
来源：http://the.fktsv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zzq.aizwys.cn

[S20] C：二分查找
来源：http://hjh.zhaomingkeji.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://azs.tianlin.xyz

[S21] C：字符类别判断
来源：http://vmi.yj20258.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sgk.jinyuanbaomall.cn

[S22] C：字符串转数字
来源：http://isr.pengpengdd.cyou

atoi("42");  strtod("3.14", NULL);
来源：http://mjn.kuanghao11.cn

[S23] C：随机数
来源：http://lhh.quarkkingdee.top

srand(time(NULL));  int r = rand() % 100;
来源：http://kda.jinqigufen.top

[S24] C：获取本地时间
来源：http://vqc.nwbrower.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qzb.ybcxt.top

[S25] C：内存拷贝
来源：http://oht.xinyue.icu

memcpy(dst, src, n);
来源：http://zzi.ivvv.top

[S26] C：内存清零
来源：http://rid.hnqzz.top

memset(a, 0, sizeof a);
来源：http://wdp.zhongyouzk.top

[S27] C：定义常量
来源：http://kye.kuanghao11.cn

const double PI = 3.14159;
来源：http://prg.hcnkem.com

[S28] C：静态变量
来源：http://nij.fengsongda.top

static int counter = 0;
来源：http://aav.jiagoushi.top

[S29] C：变参函数
来源：http://tnw.dianchejie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rai.tianlin.xyz

[S30] C：头文件保护
来源：http://xrm.shanyushiyangtech.top

#ifndef X_H
来源：http://egg.gaohongyu789.top

#define X_H
来源：http://ksw.chenzaomai.com

#endif
来源：http://vxw.yuxming.cn

[S31] C++：Hello World
来源：http://gwl.iojbl.cn

#include <iostream>
来源：http://tpe.dianchejie.cn

int main() { std::cout << "Hello\n"; }
来源：http://nad.havefunace.top

[S32] C++：字符串
来源：http://qto.nwbrower.top

std::string s = "hi";  s += "!";
来源：http://rsk.quarkkingdee.top

[S33] C++：vector 增删
来源：http://wvt.zhijiandao.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qnu.yanxiufei.cn

[S34] C++：遍历 vector
来源：http://dmp.uphjek.com

for (auto &x : v) { std::cout << x; }
来源：http://wlq.uphjek.com

[S35] C++：map
来源：http://bzg.xuetiantiany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dub.yuxming.cn

[S36] C++：unordered_map
来源：http://jwl.ctjpmb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mnp.vehdjk.com

[S37] C++：set
来源：http://glc.shangyingyoupin.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://twq.fehbvm.com

[S38] C++：排序
来源：http://zxr.pycfn.com

std::sort(v.begin(), v.end());
来源：http://ibv.sweek.top

[S39] C++：自定义比较器排序
来源：http://uss.birdmap.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eoe.sjlbkw.cn

[S40] C++：查找元素
来源：http://aob.jqgufenzy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://odc.xingfuxueyuan.xyz

[S41] C++：类与构造函数
来源：http://zqj.yj20258.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wyw.fanxiaobao.xyz

[S42] C++：继承与虚函数
来源：http://zuv.pycfn.com

class B : public Base { public: void f() override {} };
来源：http://vgv.xuanzx.com

[S43] C++：智能指针
来源：http://ckn.fehbvm.com

auto p = std::make_unique<int>(5);
来源：http://zjp.hysaishi.cn

[S44] C++：引用传参
来源：http://quu.fzhhl.top

void inc(int &x) { ++x; }
来源：http://jsx.zycfv.cn

[S45] C++：lambda
来源：http://ipz.gogol.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://dzw.gotoacloud.top

[S46] C++：函数模板
来源：http://fkk.bbcook.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cfc.kuanghao11.cn

[S47] C++：结构化绑定遍历
来源：http://zsj.feifeiyinyue.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wwy.yvedp.cn

[S48] C++：逐行读文件
来源：http://ytr.ywan-chungtsiang.top

std::ifstream in("a.txt");  std::string line;
来源：http://leo.aizwys.cn

while (std::getline(in, line)) { }
来源：http://xxq.andypj.xyz

[S49] C++：写文件
来源：http://soq.uphjek.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fge.sufxvd.cn

[S50] C++：格式化数字
来源：http://bum.jinqigfzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://toy.jianghu66.top

[S51] C++：显式类型转换
来源：http://qll.sufxvd.cn

static_cast<double>(a) / b
来源：http://tze.52xcode.cn

[S52] C++：const 与 noexcept
来源：http://rrt.ybcxt.top

int size() const noexcept { return n_; }
来源：http://xdy.nanxinkj.top

[S53] C++：移动语义
来源：http://bkj.hammf.cn

std::vector<int> w = std::move(v);
来源：http://ouv.xingfuxueyuan.xyz

[S54] C++：异常处理
来源：http://udb.shanyushiyangtech.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eko.c1oappe.top

[S55] C++：结构化绑定
来源：http://xky.feifeiyinyue.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bpp.jlsjyb.cn

[S56] C++：optional
来源：http://der.hysaishi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bbz.ivvv.top

[S57] C++：编译期常量
来源：http://rnq.bjfxy.top

constexpr int N = 10;
来源：http://tvn.yuxming.cn

[S58] C++：命名空间
来源：http://lgg.vqdsnc.cn

namespace ns { int f() { return 1; } }
来源：http://fuk.jqgufenzy.top

[S59] C++：静态断言
来源：http://ica.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gza.jyoumei.cn

[S60] C++：遍历并删除元素
来源：http://dau.gotoacloud.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pmm.yj202588.top

================================================================================
来源：http://mwj.smart0.xyz

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rhj.zhiwuduotai.top

================================================================================
来源：http://lgw.iojbl.cn

[T01] Kotlin：Hello World
来源：http://paa.xuanzx.com

println("Hello")
来源：http://yml.nanxinkj.top

[T02] Kotlin：变量
来源：http://wiu.cucudq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ssg.xylfe.cn

[T03] Kotlin：字符串模板
来源：http://oex.sxryk.cn

"值: $b"
来源：http://xct.nanxuanxn.top

[T04] Kotlin：空安全
来源：http://mor.pengpengdd.cyou

val n: String? = null;  n?.length
来源：http://oea.haohaochexian.top

[T05] Kotlin：when 表达式
来源：http://nms.redwolf501.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ksm.iojbl.cn

[T06] Kotlin：集合映射
来源：http://xhu.wangshuangyany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lah.haohaochexian.top

[T07] Kotlin：集合过滤
来源：http://dsg.daxiang520.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pse.guannengcc.top

[T08] Kotlin：数据类
来源：http://nme.hnqzz.top

data class User(val name: String, val age: Int)
来源：http://oph.havefunace.top

[T09] Kotlin：扩展函数
来源：http://zry.jyoumei.cn

fun String.exclaim() = this + "!"
来源：http://xwx.jinghuilouyu.cn

[T10] Kotlin：默认参数
来源：http://kaq.pengpengdd.cyou

fun greet(name: String = "World") = "Hi $name"
来源：http://uej.sysykeji.top

[T11] Kotlin：协程
来源：http://mni.yueranfly.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://gle.zhongyouzk.top

[T12] Kotlin：解构声明
来源：http://agh.yuanzhike.top

val (a, b) = Pair(1, 2)
来源：http://xhj.zycfv.cn

[T13] Kotlin：只读 Map
来源：http://few.meibo888.top

val m = mapOf("a" to 1)
来源：http://xux.shuidangran.top

[T14] Kotlin：循环
来源：http://ndg.52xcode.cn

for (i in 1..10) println(i)
来源：http://wax.jinghuilouyu.cn

[T15] Kotlin：接口
来源：http://gqg.sufxvd.cn

interface Shape { fun area(): Double }
来源：http://dam.jlsjyb.cn

[T16] Swift：Hello World
来源：http://jyj.hfpthk.cn

print("Hello")
来源：http://uga.wangdashe.top

[T17] Swift：变量与常量
来源：http://ots.pycfn.com

var a = 1;  let b = 2
来源：http://ymj.zhengqikj.top

[T18] Swift：字符串插值
来源：http://lxo.cheryme.top

"值: \(b)"
来源：http://muk.316326.xyz

[T19] Swift：可选绑定
来源：http://hjj.cucudq.cn

if let n = opt { print(n) }
来源：http://crz.aibaodan.cn

[T20] Swift：数组操作
来源：http://zrj.316326.xyz

var a = [1, 2, 3];  a.append(4)
来源：http://qng.epnwcf.com

[T21] Swift：遍历
来源：http://snl.hysaishi.cn

for x in a { print(x) }
来源：http://vdy.shuidangran.top

[T22] Swift：字典
来源：http://oga.nanxuanxn.top

var d = ["a": 1];  d["b"] = 2
来源：http://iou.vqdsnc.cn


<!-- 参考信息 -->