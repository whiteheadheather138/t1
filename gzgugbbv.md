代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://god.svipenyu.cn

[R14] C 风格 for
来源：http://vss.tian-w.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://urp.jyoumei.cn

[R15] while 逐行读文件
来源：http://ldi.jinyuanbaomall.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zmm.hfpthk.cn

[R16] until 等待条件
来源：http://ecy.hfpthk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gzt.ctjpmb.com

[R17] 数组定义与取值
来源：http://exv.316326.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://chf.aibaodan.cn

[R18] 遍历数组
来源：http://xqu.zhixingplan.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://byo.nanxuanxn.top

[R19] 数组长度
来源：http://svw.gzhubu.top

echo "${#arr[@]}"
来源：http://rta.xylfe.cn

[R20] 关联数组（字典）
来源：http://zaq.dianchejie.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hdr.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://tuy.xziqi.cn

echo "${#s}"
来源：http://plq.yongpay.top

[R22] 截取子串
来源：http://avm.dianchejie.cn

echo "${s:0:5}"
来源：http://hkk.xziqi.cn

[R23] 字符串替换
来源：http://ogs.hammf.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ivw.yuanzhike.top

[R24] 大小写转换
来源：http://ijc.jqgufenzy.top

echo "${s^^}"; echo "${s,,}"
来源：http://szd.ywan-chungtsiang.top

[R25] 去后缀 / 去前缀
来源：http://bki.tianlin.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://bzb.zycfv.cn

[R26] 命令替换
来源：http://xgo.wangdashe.top

now=$(date +%F); echo "$now"
来源：http://ftv.yvedp.cn

[R27] 算术展开
来源：http://ihu.xuetiantiany.cn

echo $((1 + 2 * 3))
来源：http://rti.redwolf501.top

[R28] 浮点运算
来源：http://ojm.jinghuilouyu.cn

echo "scale=2; 10/3" | bc
来源：http://vjk.haohaochexian.top

[R29] 定义函数
来源：http://zvo.cucudq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eoi.yueranfly.top

[R30] 函数返回状态码
来源：http://qgk.quarkkingdee.top

f() { return 0; }; f || echo "失败了"
来源：http://zhn.yongpay.top

[R31] 局部变量
来源：http://zgh.jinqigfzy.top

f() { local x=1; echo "$x"; }
来源：http://jsf.316326.xyz

[R32] 参数个数校验
来源：http://sfq.shanyushiyangtech.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fyf.ydjk.org.cn

[R33] 捕获错误并提示行号
来源：http://wkd.yj202588.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pwx.jqgfzy.top

[R34] 退出时清理
来源：http://hrc.yanxiufei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://cgz.xylfe.cn

[R35] 后台执行并等待
来源：http://arl.fzhhl.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mpu.52xcode.cn

[R36] 并发执行多个任务
来源：http://bdo.epnwcf.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://oho.hnxiangtu.top

[R37] 把输出赋给变量
来源：http://egx.birdmap.top

files=$(ls -1)
来源：http://rwl.nwbrower.top

[R38] 管道串联
来源：http://jgi.zhiwuduotai.top

cat a.txt | grep -i error | wc -l
来源：http://kdo.andypj.xyz

[R39] 重定向标准输出与错误
来源：http://tdp.cashguo.top

cmd > out.log 2>&1
来源：http://bmh.hnxiangtu.top

[R40] 追加写日志
来源：http://pbb.quarkkingdee.top

echo "log" >> out.log
来源：http://now.yanxiufei.cn

[R41] 丢弃输出
来源：http://jsy.cashguo.top

cmd >/dev/null 2>&1
来源：http://fis.zhijiandao.cn

[R42] 输入重定向
来源：http://jig.nanxuanxn.top

wc -l < a.txt
来源：http://hyn.ybcxt.top

[R43] 按名字查找文件
来源：http://bkx.hesvh.cn

find . -name "*.log" -type f
来源：http://xoq.tianlin.xyz

[R44] 按修改时间查找
来源：http://mmh.meibo888.top

find . -mtime -7 -type f
来源：http://uox.zdbjq.cn

[R45] 批量删除
来源：http://etv.epnwcf.com

find . -name "*.tmp" -delete
来源：http://qqj.9152youxi.cn

[R46] 递归替换文件内容
来源：http://jos.jiagoushi.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://die.yueranfly.top

[R47] sed 单行替换
来源：http://vbt.dianchejie.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ttl.sufxvd.cn

[R48] awk 取指定列
来源：http://cjd.yuanzhike.top

awk '{print $1, $3}' a.txt
来源：http://kcf.guannengcc.top

[R49] awk 带条件
来源：http://pjo.gaohongyu789.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://van.jqgufenzy.top

[R50] awk 求和
来源：http://lxw.fktsv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cpf.jinqigfzy.top

[R51] 排序去重取前几
来源：http://qor.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ayk.dianchejie.cn

[R52] 统计行数
来源：http://jhj.ywan-chungtsiang.top

wc -l a.txt
来源：http://uhc.xingfuxueyuan.xyz

[R53] 查看文件头与实时尾
来源：http://ljh.zdbjq.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vxa.shanyushiyangtech.top

[R54] 比较两个文件
来源：http://qms.cqqwz.cn

diff a.txt b.txt
来源：http://xfz.dashuyun.cn

[R55] 压缩与解压
来源：http://hjf.cashguo.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dki.yuxming.cn

[R56] 远程拷贝
来源：http://eal.birdmap.top

scp file user@host:/path/
来源：http://qho.hnqzz.top

[R57] 远程执行命令
来源：http://sik.redwolf501.top

ssh user@host 'uptime'
来源：http://bnu.tanke756.top

[R58] 下载文件
来源：http://png.quarkkingdee.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://whz.tian-w.cn

[R59] 发 POST JSON
来源：http://bzr.xuanzx.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dhg.hnqzz.top

[R60] 只看 HTTP 状态码
来源：http://tsv.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vsu.andypj.xyz

[R61] 磁盘占用
来源：http://kgq.pengpengdd.cyou

df -h;  du -sh *
来源：http://axf.jyoumei.cn

[R62] 找最占空间的文件
来源：http://sie.shuidangran.top

du -ah . | sort -rh | head -10
来源：http://wxr.redwolf501.top

[R63] 内存与进程
来源：http://brh.tarul.cn

free -h;  ps aux | grep nginx
来源：http://vqy.cqqwz.cn

[R64] 结束进程
来源：http://ial.sxryk.cn

kill -9 $(pgrep -f app.py)
来源：http://umu.tian-w.cn

[R65] 查看端口占用
来源：http://njj.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nub.jqgufenzy.top

[R66] 定时任务
来源：http://mxp.mhx1999.top

crontab -e;  crontab -l
来源：http://nmo.aibaodan.cn

[R67] 生成随机十六进制串
来源：http://yre.fengsongda.top

openssl rand -hex 16
来源：http://atn.guannengcc.top

[R68] 计算文件校验值
来源：http://ikt.52xcode.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ztm.shuidangran.top

[R69] 生成随机密码
来源：http://uys.xziqi.cn

head -c 16 /dev/urandom | base64
来源：http://slj.9152youxi.cn

[R70] 时间戳与互转
来源：http://ild.nwbrower.top

date +%s;  date -d @1700000000
来源：http://loe.andypj.xyz

[R71] 日期格式化
来源：http://teb.sxryk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qwc.sjlbkw.cn

[R72] 等待端口就绪
来源：http://dzu.nanxinkj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kqn.quarkkingdee.top

[R73] 分割大日志
来源：http://kyy.zhaomingkeji.xyz

split -l 1000 big.log part_
来源：http://zty.vqdsnc.cn

[R74] 批量重命名
来源：http://cku.nanxuanxn.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iaf.zhixingplan.top

[R75] 导出环境变量
来源：http://izn.aibaodan.cn

export PATH="$HOME/bin:$PATH"
来源：http://otc.iojbl.cn

[R76] 使用临时文件
来源：http://gvl.cdnleiting.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ozf.cdnleiting.top

[R77] 读取用户输入
来源：http://gcd.cashguo.top

read -rp "请输入: " ans
来源：http://xjl.pengpengdd.cyou

[R78] 交互式菜单
来源：http://lsd.iojbl.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ygt.ehwqpu.com

[R79] 解析命令行选项
来源：http://qel.gotoacloud.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jsr.chenzaomai.com

[R80] 查看脚本执行耗时
来源：http://eli.nanxuanxn.top

time ./run.sh
来源：http://loz.yuxming.cn

================================================================================
来源：http://wgb.dianchejie.cn

S. C / C++ 专题
来源：http://owl.mhx1999.top

================================================================================
来源：http://nzy.xziqi.cn

[S01] C：Hello World
来源：http://cdh.ywan-chungtsiang.top

#include <stdio.h>
来源：http://bxe.hammf.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qek.shuidangran.top

[S02] C：变量与格式化输出
来源：http://ity.snrcjt.cn

int a = 10; printf("%d\n", a);
来源：http://csg.ydjk.org.cn

[S03] C：读入整数
来源：http://avu.yanxiufei.cn

int x; scanf("%d", &x);
来源：http://qna.birdmap.top

[S04] C：字符串复制
来源：http://psu.pengpengdd.cyou

char dst[32]; strcpy(dst, "hi");
来源：http://hxr.nwbrower.top

[S05] C：字符串长度
来源：http://ixv.redwolf501.top

strlen(s)
来源：http://knc.feifeiyinyue.top

[S06] C：字符串比较
来源：http://dmr.smart0.xyz

strcmp(a, b) == 0
来源：http://uok.yuxming.cn

[S07] C：数组遍历求和
来源：http://sip.ehwqpu.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://huv.shanyushiyangtech.top

[S08] C：动态内存分配与释放
来源：http://kan.fktsv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vaf.ydjk.org.cn

[S09] C：结构体定义与初始化
来源：http://zww.jlsjyb.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gok.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://uol.gogol.net.cn

int *p = &a;  *p = 5;
来源：http://thl.vqdsnc.cn

[S11] C：逐行读文件
来源：http://slq.zdqjudy.top

FILE *f = fopen("a.txt", "r");
来源：http://kqd.jinyuanbaomall.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tbo.ppjwa.cn

fclose(f);
来源：http://olr.jinqigufen.top

[S12] C：写文件
来源：http://alr.vqdsnc.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ape.yangfankeji.com

[S13] C：宏定义
来源：http://wwc.meibo888.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qyu.9152youxi.cn

[S14] C：枚举
来源：http://xye.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://wjr.hfpthk.cn

[S15] C：类型转换
来源：http://bcb.nanxuanxn.top

(double) a / b
来源：http://lgq.hnqzz.top

[S16] C：位操作置位
来源：http://tec.xziqi.cn

x |= (1 << 3);
来源：http://xwm.cashguo.top

[S17] C：安全拼接字符串
来源：http://fwx.yuxming.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kuy.fengsongda.top

[S18] C：命令行参数
来源：http://dyz.yfazqb.com

int main(int argc, char **argv)
来源：http://jmc.yuxming.cn

[S19] C：快速排序
来源：http://ivj.sweek.top

qsort(a, n, sizeof(int), cmp);
来源：http://buj.zhaomingkeji.xyz

[S20] C：二分查找
来源：http://ayz.feifeiyinyue.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xtu.tarul.cn

[S21] C：字符类别判断
来源：http://gzv.sysykeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://flr.bjfxy.top

[S22] C：字符串转数字
来源：http://afy.gzhubu.top

atoi("42");  strtod("3.14", NULL);
来源：http://opv.zycfv.cn

[S23] C：随机数
来源：http://fge.wangshuangyany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kzp.gzhubu.top

[S24] C：获取本地时间
来源：http://vcr.pycfn.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qbi.cqqwz.cn

[S25] C：内存拷贝
来源：http://hna.ehwqpu.com

memcpy(dst, src, n);
来源：http://kvr.uphjek.com

[S26] C：内存清零
来源：http://kfx.hongshengwenyu.top

memset(a, 0, sizeof a);
来源：http://yqi.ehwqpu.com

[S27] C：定义常量
来源：http://znr.nanxinkj.top

const double PI = 3.14159;
来源：http://iyr.sysykeji.top

[S28] C：静态变量
来源：http://kle.zhoulong.xyz

static int counter = 0;
来源：http://pox.xinyue.icu

[S29] C：变参函数
来源：http://lrm.feifeiyinyue.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://jel.haohaochexian.top

[S30] C：头文件保护
来源：http://sxd.tanke756.top

#ifndef X_H
来源：http://trm.yj20258.top

#define X_H
来源：http://xhw.meibo888.top

#endif
来源：http://zrp.zhengqikj.top

[S31] C++：Hello World
来源：http://kmk.wangshuangyany.cn

#include <iostream>
来源：http://nye.zhengqikj.top

int main() { std::cout << "Hello\n"; }
来源：http://dan.yuxming.cn

[S32] C++：字符串
来源：http://hoc.jlsjyb.cn

std::string s = "hi";  s += "!";
来源：http://rtn.cqqwz.cn

[S33] C++：vector 增删
来源：http://rbn.fengsongda.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://klz.nanxuanxn.top

[S34] C++：遍历 vector
来源：http://xbt.cucudq.cn

for (auto &x : v) { std::cout << x; }
来源：http://dqt.cdnleiting.top

[S35] C++：map
来源：http://tnc.dianchejie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yoi.birdmap.top

[S36] C++：unordered_map
来源：http://jjd.haohaochexian.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bsi.zdbjq.cn

[S37] C++：set
来源：http://vvi.vehdjk.com

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sjw.chenjidiqi.icu

[S38] C++：排序
来源：http://zqo.yangfankeji.com

std::sort(v.begin(), v.end());
来源：http://gwx.feifeiyinyue.top

[S39] C++：自定义比较器排序
来源：http://lyh.nwbrower.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xbk.nanxinkj.top

[S40] C++：查找元素
来源：http://iuu.zdqjudy.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sjp.zhixingplan.top

[S41] C++：类与构造函数
来源：http://ngv.bbcook.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://myk.xylfe.cn

[S42] C++：继承与虚函数
来源：http://tzs.yueranfly.top

class B : public Base { public: void f() override {} };
来源：http://dsl.svipenyu.cn

[S43] C++：智能指针
来源：http://zvh.bbcook.cn

auto p = std::make_unique<int>(5);
来源：http://eth.shanyushiyangtech.top

[S44] C++：引用传参
来源：http://dln.c1oappe.top

void inc(int &x) { ++x; }
来源：http://ulh.epnwcf.com

[S45] C++：lambda
来源：http://zvr.tianlin.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://mre.ywan-chungtsiang.top

[S46] C++：函数模板
来源：http://aam.zhongyouzk.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ygb.zhengqikj.top

[S47] C++：结构化绑定遍历
来源：http://aed.yfazqb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yxw.ppjwa.cn

[S48] C++：逐行读文件
来源：http://gyq.sysykeji.top

std::ifstream in("a.txt");  std::string line;
来源：http://hfb.cdnleiting.top

while (std::getline(in, line)) { }
来源：http://lhq.shanyushiyangkeji.top

[S49] C++：写文件
来源：http://buq.smart0.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://phf.pycfn.com

[S50] C++：格式化数字
来源：http://zkh.zhoulong.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ouc.yuxming.cn

[S51] C++：显式类型转换
来源：http://elq.daria6918.cn

static_cast<double>(a) / b
来源：http://abm.dianchejie.cn

[S52] C++：const 与 noexcept
来源：http://iiv.fengsongda.top

int size() const noexcept { return n_; }
来源：http://vzq.c1oappe.top

[S53] C++：移动语义
来源：http://gez.jqgfzy.top

std::vector<int> w = std::move(v);
来源：http://kse.jlsjyb.cn

[S54] C++：异常处理
来源：http://hyk.feifeiyinyue.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://udb.zhijiandao.cn

[S55] C++：结构化绑定
来源：http://gbb.yuxming.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cyo.vehdjk.com

[S56] C++：optional
来源：http://ugm.nanxinkj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://eob.zdqjudy.top

[S57] C++：编译期常量
来源：http://qiv.fktsv.cn

constexpr int N = 10;
来源：http://iqd.ywan-chungtsiang.top

[S58] C++：命名空间
来源：http://ykk.yfazqb.com

namespace ns { int f() { return 1; } }
来源：http://qff.shzxlz.cn

[S59] C++：静态断言
来源：http://jui.yanxiufei.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tvu.yj20258888.top

[S60] C++：遍历并删除元素
来源：http://hfr.316326.xyz

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eyi.zhixingplan.top

================================================================================
来源：http://dan.zhijiandao.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jcl.dianchejie.cn

================================================================================
来源：http://ify.daxiang520.top

[T01] Kotlin：Hello World
来源：http://qig.tian-w.cn

println("Hello")
来源：http://owi.birdmap.top

[T02] Kotlin：变量
来源：http://vug.tarul.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vfd.xylfe.cn

[T03] Kotlin：字符串模板
来源：http://amy.vqdsnc.cn

"值: $b"
来源：http://wls.cashguo.top

[T04] Kotlin：空安全
来源：http://fhx.zhixingplan.top

val n: String? = null;  n?.length
来源：http://rpq.ctjpmb.com

[T05] Kotlin：when 表达式
来源：http://epn.fzhhl.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://veb.jqgfzy.top

[T06] Kotlin：集合映射
来源：http://yjt.sjlbkw.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vys.hnqzz.top

[T07] Kotlin：集合过滤
来源：http://itb.jqgfzy.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://xfb.daria6918.cn

[T08] Kotlin：数据类
来源：http://tmv.fzhhl.top

data class User(val name: String, val age: Int)
来源：http://koj.gotoacloud.top

[T09] Kotlin：扩展函数
来源：http://kel.gogol.net.cn

fun String.exclaim() = this + "!"
来源：http://jtg.sufxvd.cn

[T10] Kotlin：默认参数
来源：http://mfo.shuidangran.top

fun greet(name: String = "World") = "Hi $name"
来源：http://sdp.yj202588.top

[T11] Kotlin：协程
来源：http://qxn.nwbrower.top

GlobalScope.launch { delay(1000); println("done") }
来源：http://xyr.zhixingplan.top

[T12] Kotlin：解构声明
来源：http://tqw.wangdashe.top

val (a, b) = Pair(1, 2)
来源：http://awv.sjlbkw.cn

[T13] Kotlin：只读 Map
来源：http://php.hcnkem.com

val m = mapOf("a" to 1)
来源：http://oeh.sxryk.cn

[T14] Kotlin：循环
来源：http://pgc.jqgufenzy.top

for (i in 1..10) println(i)
来源：http://nyw.ehwqpu.com

[T15] Kotlin：接口
来源：http://jkc.aibaodan.cn

interface Shape { fun area(): Double }
来源：http://stb.fanxiaobao.xyz

[T16] Swift：Hello World
来源：http://cgx.jyoumei.cn

print("Hello")
来源：http://jjm.nanxuanxn.top


<!-- 参考信息 -->