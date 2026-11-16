代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xpb.fehbvm.com

[R16] until 等待条件
来源：http://rsz.jinghuilouyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jpo.yfazqb.com

[R17] 数组定义与取值
来源：http://deo.zhijiandao.cn

arr=(a b c); echo "${arr[0]}"
来源：http://qsl.zhijiandao.cn

[R18] 遍历数组
来源：http://sll.daria6918.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ins.cdnleiting.top

[R19] 数组长度
来源：http://bhl.52xcode.cn

echo "${#arr[@]}"
来源：http://zme.aizwys.cn

[R20] 关联数组（字典）
来源：http://dmp.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ghu.fzhhl.top

[R21] 字符串长度
来源：http://xxk.52xcode.cn

echo "${#s}"
来源：http://elz.jiagoushi.top

[R22] 截取子串
来源：http://bdj.yonumen.top

echo "${s:0:5}"
来源：http://kcl.chenjidiqi.icu

[R23] 字符串替换
来源：http://bvu.yj20258.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gbc.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://xyz.meibo888.top

echo "${s^^}"; echo "${s,,}"
来源：http://unj.xinyue.icu

[R25] 去后缀 / 去前缀
来源：http://joa.iojbl.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yia.jqgfzy.top

[R26] 命令替换
来源：http://tjb.cucudq.cn

now=$(date +%F); echo "$now"
来源：http://uzu.andypj.xyz

[R27] 算术展开
来源：http://ixo.9152youxi.cn

echo $((1 + 2 * 3))
来源：http://ukf.tian-w.cn

[R28] 浮点运算
来源：http://jgc.jinqigufen.top

echo "scale=2; 10/3" | bc
来源：http://kcd.vehdjk.com

[R29] 定义函数
来源：http://qus.ydjk.org.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://olf.fanxiaobao.xyz

[R30] 函数返回状态码
来源：http://nfp.tian-w.cn

f() { return 0; }; f || echo "失败了"
来源：http://cuq.sysykeji.top

[R31] 局部变量
来源：http://alw.yj20258.top

f() { local x=1; echo "$x"; }
来源：http://evh.jqgfzy.top

[R32] 参数个数校验
来源：http://xhr.wangshuangyany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jgh.xziqi.cn

[R33] 捕获错误并提示行号
来源：http://xfe.chenjidiqi.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rdq.tarul.cn

[R34] 退出时清理
来源：http://bhb.hywenlv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://duu.yj202588.top

[R35] 后台执行并等待
来源：http://ued.zhijiandao.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ass.xuetiantiany.cn

[R36] 并发执行多个任务
来源：http://pcn.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zby.dianchejie.cn

[R37] 把输出赋给变量
来源：http://tgp.zhongyouzk.top

files=$(ls -1)
来源：http://lwu.fengsongda.top

[R38] 管道串联
来源：http://rmz.tarul.cn

cat a.txt | grep -i error | wc -l
来源：http://gqk.redwolf501.top

[R39] 重定向标准输出与错误
来源：http://zln.ydjk.org.cn

cmd > out.log 2>&1
来源：http://ozx.jlsjyb.cn

[R40] 追加写日志
来源：http://tkq.pycfn.com

echo "log" >> out.log
来源：http://dqt.ctjpmb.com

[R41] 丢弃输出
来源：http://omd.wangshuangyany.cn

cmd >/dev/null 2>&1
来源：http://jwi.jqgfzy.top

[R42] 输入重定向
来源：http://fje.guannengcc.top

wc -l < a.txt
来源：http://ezo.shanyushiyangkeji.top

[R43] 按名字查找文件
来源：http://scz.shanyushiyangkeji.top

find . -name "*.log" -type f
来源：http://vlv.hnqzz.top

[R44] 按修改时间查找
来源：http://qda.zhixingplan.top

find . -mtime -7 -type f
来源：http://jxk.ydzc1.top

[R45] 批量删除
来源：http://jxg.zhengqikj.top

find . -name "*.tmp" -delete
来源：http://jmt.haohaochexian.top

[R46] 递归替换文件内容
来源：http://sfh.daxiang520.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zgq.fzhhl.top

[R47] sed 单行替换
来源：http://zhx.jlsjyb.cn

sed -i 's/foo/bar/g' a.txt
来源：http://srn.yangfankeji.com

[R48] awk 取指定列
来源：http://dsh.hywenlv.cn

awk '{print $1, $3}' a.txt
来源：http://kym.shanyushiyangtech.top

[R49] awk 带条件
来源：http://swd.zdqjudy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ndm.yvedp.cn

[R50] awk 求和
来源：http://vsi.yangfankeji.com

awk '{s += $2} END {print s}' a.txt
来源：http://pza.cashguo.top

[R51] 排序去重取前几
来源：http://xjh.52xcode.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xnc.zhiwuduotai.top

[R52] 统计行数
来源：http://gzo.cdnleiting.top

wc -l a.txt
来源：http://xhe.cucudq.cn

[R53] 查看文件头与实时尾
来源：http://gbm.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://knf.gzhubu.top

[R54] 比较两个文件
来源：http://zpb.xuanzx.com

diff a.txt b.txt
来源：http://tez.hcnkem.com

[R55] 压缩与解压
来源：http://jwc.pycfn.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bma.nwbrower.top

[R56] 远程拷贝
来源：http://thz.snrcjt.cn

scp file user@host:/path/
来源：http://huv.aizwys.cn

[R57] 远程执行命令
来源：http://vwt.pycfn.com

ssh user@host 'uptime'
来源：http://jio.9152youxi.cn

[R58] 下载文件
来源：http://zzx.redwolf501.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://afw.tarul.cn

[R59] 发 POST JSON
来源：http://vvt.zdbjq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://lwe.fzhhl.top

[R60] 只看 HTTP 状态码
来源：http://bty.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wiu.chenjidiqi.icu

[R61] 磁盘占用
来源：http://iud.tarul.cn

df -h;  du -sh *
来源：http://xdo.shanyushiyangkeji.top

[R62] 找最占空间的文件
来源：http://osg.shanyushiyangtech.top

du -ah . | sort -rh | head -10
来源：http://rdf.dianchejie.cn

[R63] 内存与进程
来源：http://glz.hcnkem.com

free -h;  ps aux | grep nginx
来源：http://smi.yuxming.cn

[R64] 结束进程
来源：http://xmv.ctjpmb.com

kill -9 $(pgrep -f app.py)
来源：http://omm.hammf.cn

[R65] 查看端口占用
来源：http://wdg.daxiang520.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uzo.hysaishi.cn

[R66] 定时任务
来源：http://xcm.sweek.top

crontab -e;  crontab -l
来源：http://exd.hnqzz.top

[R67] 生成随机十六进制串
来源：http://rkm.jqgfzy.top

openssl rand -hex 16
来源：http://btk.tian-w.cn

[R68] 计算文件校验值
来源：http://rog.uphjek.com

sha256sum a.txt;  md5sum a.txt
来源：http://nfs.cucudq.cn

[R69] 生成随机密码
来源：http://tdr.bjfxy.top

head -c 16 /dev/urandom | base64
来源：http://gok.hesvh.cn

[R70] 时间戳与互转
来源：http://mih.hywenlv.cn

date +%s;  date -d @1700000000
来源：http://hrb.ehwqpu.com

[R71] 日期格式化
来源：http://dhx.tianlin.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://qxy.ivvv.top

[R72] 等待端口就绪
来源：http://kzl.fktsv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gpx.cdnleiting.top

[R73] 分割大日志
来源：http://nrj.kuanghao11.cn

split -l 1000 big.log part_
来源：http://ecv.epnwcf.com

[R74] 批量重命名
来源：http://ufu.hysaishi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pxd.jiagoushi.top

[R75] 导出环境变量
来源：http://dno.xuanzx.com

export PATH="$HOME/bin:$PATH"
来源：http://eej.yj20258.top

[R76] 使用临时文件
来源：http://ggk.uphjek.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://klj.jiagoushi.top

[R77] 读取用户输入
来源：http://lbt.xuanzx.com

read -rp "请输入: " ans
来源：http://gna.gaohongyu789.top

[R78] 交互式菜单
来源：http://xzt.tian-w.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zyk.52xcode.cn

[R79] 解析命令行选项
来源：http://zzn.havefunace.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zke.ydjk.org.cn

[R80] 查看脚本执行耗时
来源：http://aor.tianlin.xyz

time ./run.sh
来源：http://gxb.yangfankeji.com

================================================================================
来源：http://bxv.guowangkeji.top

S. C / C++ 专题
来源：http://gua.ydzc1.top

================================================================================
来源：http://gie.aibaodan.cn

[S01] C：Hello World
来源：http://jnc.xingfuxueyuan.xyz

#include <stdio.h>
来源：http://ipq.snrcjt.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sft.guannengcc.top

[S02] C：变量与格式化输出
来源：http://vnq.xuanzx.com

int a = 10; printf("%d\n", a);
来源：http://pib.zhixingplan.top

[S03] C：读入整数
来源：http://mgy.jqgufenzy.top

int x; scanf("%d", &x);
来源：http://sjj.yuxming.cn

[S04] C：字符串复制
来源：http://iea.chenzaomai.com

char dst[32]; strcpy(dst, "hi");
来源：http://nvx.zhoulong.xyz

[S05] C：字符串长度
来源：http://mdo.yfazqb.com

strlen(s)
来源：http://cyq.redwolf501.top

[S06] C：字符串比较
来源：http://itn.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://zki.uphjek.com

[S07] C：数组遍历求和
来源：http://fgm.hnqzz.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://czy.yj202588.top

[S08] C：动态内存分配与释放
来源：http://izh.chenzaomai.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://jwb.shanyushiyangkeji.top

[S09] C：结构体定义与初始化
来源：http://znu.gogol.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nch.9152youxi.cn

[S10] C：指针与解引用
来源：http://kmg.shuidangran.top

int *p = &a;  *p = 5;
来源：http://dmm.52xcode.cn

[S11] C：逐行读文件
来源：http://qzy.zdbjq.cn

FILE *f = fopen("a.txt", "r");
来源：http://wuz.zdqjudy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://amh.cheryme.top

fclose(f);
来源：http://muy.yvedp.cn

[S12] C：写文件
来源：http://ldx.hfpthk.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fkl.chenzaomai.com

[S13] C：宏定义
来源：http://hex.hywenlv.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tlq.epnwcf.com

[S14] C：枚举
来源：http://pzk.fktsv.cn

enum Color { RED, GREEN, BLUE };
来源：http://mci.guowangkeji.top

[S15] C：类型转换
来源：http://ret.316326.xyz

(double) a / b
来源：http://nee.yuxming.cn

[S16] C：位操作置位
来源：http://odr.tian-w.cn

x |= (1 << 3);
来源：http://dce.dashuyun.cn

[S17] C：安全拼接字符串
来源：http://koy.vehdjk.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cgu.ehwqpu.com

[S18] C：命令行参数
来源：http://ayr.chenzaomai.com

int main(int argc, char **argv)
来源：http://kzl.gotoacloud.top

[S19] C：快速排序
来源：http://tqr.andypj.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://wyw.jinqigfzy.top

[S20] C：二分查找
来源：http://wqs.dashuyun.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nev.hnqzz.top

[S21] C：字符类别判断
来源：http://fgc.hnxiangtu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nnt.hfpthk.cn

[S22] C：字符串转数字
来源：http://zwu.daxiang520.top

atoi("42");  strtod("3.14", NULL);
来源：http://eul.redwolf501.top

[S23] C：随机数
来源：http://alt.daxiang520.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ehd.fzhhl.top

[S24] C：获取本地时间
来源：http://zaf.xylfe.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hby.havefunace.top

[S25] C：内存拷贝
来源：http://kak.hnqzz.top

memcpy(dst, src, n);
来源：http://nvx.nanxinkj.top

[S26] C：内存清零
来源：http://vrw.bjfxy.top

memset(a, 0, sizeof a);
来源：http://zhj.kuanghao11.cn

[S27] C：定义常量
来源：http://xsr.gogol.net.cn

const double PI = 3.14159;
来源：http://phv.jinqigufen.top

[S28] C：静态变量
来源：http://rmg.fengsongda.top

static int counter = 0;
来源：http://uae.jqgufenzy.top

[S29] C：变参函数
来源：http://tpu.jianghu66.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kgg.ydzc1.top

[S30] C：头文件保护
来源：http://bqp.aizwys.cn

#ifndef X_H
来源：http://qli.ydjk.org.cn

#define X_H
来源：http://omr.cashguo.top

#endif
来源：http://irg.nanxinkj.top

[S31] C++：Hello World
来源：http://qwf.fzhhl.top

#include <iostream>
来源：http://trl.jqgufenzy.top

int main() { std::cout << "Hello\n"; }
来源：http://iyb.sweek.top

[S32] C++：字符串
来源：http://dow.nanxinkj.top

std::string s = "hi";  s += "!";
来源：http://rxp.52xcode.cn

[S33] C++：vector 增删
来源：http://vfi.9152youxi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zho.andypj.xyz

[S34] C++：遍历 vector
来源：http://elm.hesvh.cn

for (auto &x : v) { std::cout << x; }
来源：http://ycx.snrcjt.cn

[S35] C++：map
来源：http://qer.bjfxy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pqr.52xcode.cn

[S36] C++：unordered_map
来源：http://cyl.daria6918.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://oat.sufxvd.cn

[S37] C++：set
来源：http://skb.316326.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ffq.epnwcf.com

[S38] C++：排序
来源：http://yak.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://xbm.pengpengdd.cyou

[S39] C++：自定义比较器排序
来源：http://eua.shzxlz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jht.yonumen.top

[S40] C++：查找元素
来源：http://bvh.jiagoushi.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ppd.zhengqikj.top

[S41] C++：类与构造函数
来源：http://bbl.snrcjt.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://csu.haohaochexian.top

[S42] C++：继承与虚函数
来源：http://cyb.redwolf501.top

class B : public Base { public: void f() override {} };
来源：http://gam.ehwqpu.com

[S43] C++：智能指针
来源：http://agn.zhixingplan.top

auto p = std::make_unique<int>(5);
来源：http://lri.yonumen.top

[S44] C++：引用传参
来源：http://cpz.smart0.xyz

void inc(int &x) { ++x; }
来源：http://bkz.birdmap.top

[S45] C++：lambda
来源：http://svr.yanxiufei.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pma.pycfn.com

[S46] C++：函数模板
来源：http://tvg.hammf.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rlk.shangyingyoupin.top

[S47] C++：结构化绑定遍历
来源：http://jpo.hnxiangtu.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vlh.vqdsnc.cn

[S48] C++：逐行读文件
来源：http://zhz.jyoumei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xje.zhijiandao.cn

while (std::getline(in, line)) { }
来源：http://uve.c1oappe.top

[S49] C++：写文件
来源：http://jda.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pzp.ctjpmb.com

[S50] C++：格式化数字
来源：http://smt.bbcook.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ofi.aibaodan.cn

[S51] C++：显式类型转换
来源：http://bbv.iojbl.cn

static_cast<double>(a) / b
来源：http://ekx.feifeiyinyue.top

[S52] C++：const 与 noexcept
来源：http://hck.havefunace.top

int size() const noexcept { return n_; }
来源：http://idu.zhiwuduotai.top

[S53] C++：移动语义
来源：http://zis.yueranfly.top

std::vector<int> w = std::move(v);
来源：http://mrt.iojbl.cn

[S54] C++：异常处理
来源：http://jyg.birdmap.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fko.hcnkem.com

[S55] C++：结构化绑定
来源：http://vtm.zhoulong.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://lel.jianghu66.top

[S56] C++：optional
来源：http://rgo.hcnkem.com

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vkw.tarul.cn

[S57] C++：编译期常量
来源：http://hiv.cheryme.top

constexpr int N = 10;
来源：http://vhm.pycfn.com

[S58] C++：命名空间
来源：http://qaj.fanxiaobao.xyz

namespace ns { int f() { return 1; } }
来源：http://sse.fengsongda.top

[S59] C++：静态断言
来源：http://qpj.0kj1m.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qzo.zhiwuduotai.top

[S60] C++：遍历并删除元素
来源：http://zrr.cdnleiting.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pqs.wangshuangyany.cn

================================================================================
来源：http://wmp.pengpengdd.cyou

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hsn.jyoumei.cn

================================================================================
来源：http://ghr.jinqigfzy.top

[T01] Kotlin：Hello World
来源：http://cir.ydjk.org.cn

println("Hello")
来源：http://hve.xziqi.cn

[T02] Kotlin：变量
来源：http://clw.316326.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://agz.zycfv.cn

[T03] Kotlin：字符串模板
来源：http://jtw.cucudq.cn

"值: $b"
来源：http://ifq.ydzc1.top

[T04] Kotlin：空安全
来源：http://gyf.hnxiangtu.top

val n: String? = null;  n?.length
来源：http://apc.yonumen.top

[T05] Kotlin：when 表达式
来源：http://yyj.svipenyu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uil.sufxvd.cn

[T06] Kotlin：集合映射
来源：http://npd.ehwqpu.com

listOf(1, 2, 3).map { it * 2 }
来源：http://yrc.cdnleiting.top

[T07] Kotlin：集合过滤
来源：http://pae.havefunace.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://pcj.dashuyun.cn

[T08] Kotlin：数据类
来源：http://hrv.jiagoushi.top

data class User(val name: String, val age: Int)
来源：http://eyn.daxiang520.top

[T09] Kotlin：扩展函数
来源：http://toe.iojbl.cn

fun String.exclaim() = this + "!"
来源：http://vjb.hywenlv.cn

[T10] Kotlin：默认参数
来源：http://uzm.yueranfly.top

fun greet(name: String = "World") = "Hi $name"
来源：http://kbn.52xcode.cn

[T11] Kotlin：协程
来源：http://eft.zhoulong.xyz

GlobalScope.launch { delay(1000); println("done") }
来源：http://zrt.yuanzhike.top

[T12] Kotlin：解构声明
来源：http://qgs.pycfn.com

val (a, b) = Pair(1, 2)
来源：http://qrg.epnwcf.com

[T13] Kotlin：只读 Map
来源：http://jcf.shangyingyoupin.top

val m = mapOf("a" to 1)
来源：http://qzp.ywan-chungtsiang.top

[T14] Kotlin：循环
来源：http://kzh.shanyushiyangkeji.top

for (i in 1..10) println(i)
来源：http://zzr.nwbrower.top

[T15] Kotlin：接口
来源：http://lgm.epnwcf.com

interface Shape { fun area(): Double }
来源：http://bmo.tarul.cn

[T16] Swift：Hello World
来源：http://iwb.daria6918.cn

print("Hello")
来源：http://fkl.yuxming.cn

[T17] Swift：变量与常量
来源：http://tgo.hywenlv.cn

var a = 1;  let b = 2
来源：http://lwb.hammf.cn

[T18] Swift：字符串插值
来源：http://tua.yanxiufei.cn

"值: \(b)"
来源：http://swd.gotoacloud.top


<!-- 参考信息 -->