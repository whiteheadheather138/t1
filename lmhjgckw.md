代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xco.gaohongyu789.top

[R16] until 等待条件
来源：http://oxu.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xic.ehwqpu.com

[R17] 数组定义与取值
来源：http://sfw.zhengqikj.top

arr=(a b c); echo "${arr[0]}"
来源：http://xmb.pycfn.com

[R18] 遍历数组
来源：http://tvr.xylfe.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gge.zdqjudy.top

[R19] 数组长度
来源：http://zki.tanke756.top

echo "${#arr[@]}"
来源：http://val.guowangkeji.top

[R20] 关联数组（字典）
来源：http://qdo.yueranfly.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://csn.wangshuangyany.cn

[R21] 字符串长度
来源：http://ltt.cqqwz.cn

echo "${#s}"
来源：http://rns.gzhubu.top

[R22] 截取子串
来源：http://qan.shanyushiyangkeji.top

echo "${s:0:5}"
来源：http://cyk.hywenlv.cn

[R23] 字符串替换
来源：http://apw.pengpengdd.cyou

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ykf.zhoulong.xyz

[R24] 大小写转换
来源：http://mnu.gzhubu.top

echo "${s^^}"; echo "${s,,}"
来源：http://wer.zhoulong.xyz

[R25] 去后缀 / 去前缀
来源：http://ufe.tianlin.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://pkz.aizwys.cn

[R26] 命令替换
来源：http://kzj.9152youxi.cn

now=$(date +%F); echo "$now"
来源：http://gfp.xingfuxueyuan.xyz

[R27] 算术展开
来源：http://dbw.hnxiangtu.top

echo $((1 + 2 * 3))
来源：http://bqj.xinyue.icu

[R28] 浮点运算
来源：http://fby.jiagoushi.top

echo "scale=2; 10/3" | bc
来源：http://eiz.daxiang520.top

[R29] 定义函数
来源：http://mms.zhaomingkeji.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ynr.zhoulong.xyz

[R30] 函数返回状态码
来源：http://guj.ctjpmb.com

f() { return 0; }; f || echo "失败了"
来源：http://ssx.zhoulong.xyz

[R31] 局部变量
来源：http://jpo.gaohongyu789.top

f() { local x=1; echo "$x"; }
来源：http://qfp.aibaodan.cn

[R32] 参数个数校验
来源：http://pdq.xylfe.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mho.tanke756.top

[R33] 捕获错误并提示行号
来源：http://srt.xinyue.icu

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mbi.chenjidiqi.icu

[R34] 退出时清理
来源：http://rqf.pycfn.com

trap 'rm -f "$tmp"' EXIT
来源：http://syq.gaohongyu789.top

[R35] 后台执行并等待
来源：http://wip.hfpthk.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://imr.bbcook.cn

[R36] 并发执行多个任务
来源：http://otf.sjlbkw.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zot.sufxvd.cn

[R37] 把输出赋给变量
来源：http://mgz.sxryk.cn

files=$(ls -1)
来源：http://ztu.yanxiufei.cn

[R38] 管道串联
来源：http://ooz.zhijiandao.cn

cat a.txt | grep -i error | wc -l
来源：http://cpl.zdbjq.cn

[R39] 重定向标准输出与错误
来源：http://pcm.kuanghao11.cn

cmd > out.log 2>&1
来源：http://kld.vqdsnc.cn

[R40] 追加写日志
来源：http://lrb.nwbrower.top

echo "log" >> out.log
来源：http://wgo.0kj1m.cn

[R41] 丢弃输出
来源：http://kbb.vehdjk.com

cmd >/dev/null 2>&1
来源：http://dmm.tianlin.xyz

[R42] 输入重定向
来源：http://ypu.shuidangran.top

wc -l < a.txt
来源：http://fxz.hnxiangtu.top

[R43] 按名字查找文件
来源：http://mku.yuxming.cn

find . -name "*.log" -type f
来源：http://ssg.havefunace.top

[R44] 按修改时间查找
来源：http://vnf.xinyue.icu

find . -mtime -7 -type f
来源：http://bts.tian-w.cn

[R45] 批量删除
来源：http://kmj.tian-w.cn

find . -name "*.tmp" -delete
来源：http://ose.wangdashe.top

[R46] 递归替换文件内容
来源：http://whh.pycfn.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nyo.jinyuanbaomall.cn

[R47] sed 单行替换
来源：http://reh.sxryk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tcv.jqgufenzy.top

[R48] awk 取指定列
来源：http://xye.sysykeji.top

awk '{print $1, $3}' a.txt
来源：http://dvd.jiagoushi.top

[R49] awk 带条件
来源：http://cga.hfpthk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://agn.iojbl.cn

[R50] awk 求和
来源：http://mhq.yj202588.top

awk '{s += $2} END {print s}' a.txt
来源：http://wcy.gotoacloud.top

[R51] 排序去重取前几
来源：http://ffs.xziqi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fjt.ctjpmb.com

[R52] 统计行数
来源：http://fku.yj20258888.top

wc -l a.txt
来源：http://xfo.fktsv.cn

[R53] 查看文件头与实时尾
来源：http://jdf.zhaomingkeji.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jfl.gogol.net.cn

[R54] 比较两个文件
来源：http://gvt.316326.xyz

diff a.txt b.txt
来源：http://iwk.jianghu66.top

[R55] 压缩与解压
来源：http://jyv.meibo888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cua.xinyue.icu

[R56] 远程拷贝
来源：http://fzq.daxiang520.top

scp file user@host:/path/
来源：http://jyv.zhoulong.xyz

[R57] 远程执行命令
来源：http://trq.fengsongda.top

ssh user@host 'uptime'
来源：http://vwe.bjfxy.top

[R58] 下载文件
来源：http://ure.yj202588.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lpb.iojbl.cn

[R59] 发 POST JSON
来源：http://mlp.c1oappe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rmv.zycfv.cn

[R60] 只看 HTTP 状态码
来源：http://vbj.hesvh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://inj.fktsv.cn

[R61] 磁盘占用
来源：http://nko.fanxiaobao.xyz

df -h;  du -sh *
来源：http://bie.fktsv.cn

[R62] 找最占空间的文件
来源：http://qkw.hysaishi.cn

du -ah . | sort -rh | head -10
来源：http://lul.chenzaomai.com

[R63] 内存与进程
来源：http://chx.hcnkem.com

free -h;  ps aux | grep nginx
来源：http://nfu.cucudq.cn

[R64] 结束进程
来源：http://tdl.pengpengdd.cyou

kill -9 $(pgrep -f app.py)
来源：http://fyq.zhongyouzk.top

[R65] 查看端口占用
来源：http://dss.aibaodan.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://iru.xuanzx.com

[R66] 定时任务
来源：http://ceh.tian-w.cn

crontab -e;  crontab -l
来源：http://ngx.hammf.cn

[R67] 生成随机十六进制串
来源：http://ibt.hfpthk.cn

openssl rand -hex 16
来源：http://rnb.havefunace.top

[R68] 计算文件校验值
来源：http://wtj.nanxinkj.top

sha256sum a.txt;  md5sum a.txt
来源：http://sbx.fengsongda.top

[R69] 生成随机密码
来源：http://ill.yj20258888.top

head -c 16 /dev/urandom | base64
来源：http://etm.sysykeji.top

[R70] 时间戳与互转
来源：http://quc.epnwcf.com

date +%s;  date -d @1700000000
来源：http://hcr.ppjwa.cn

[R71] 日期格式化
来源：http://hza.shuidangran.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kgi.sjlbkw.cn

[R72] 等待端口就绪
来源：http://ayt.shangyingyoupin.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fdg.xylfe.cn

[R73] 分割大日志
来源：http://faq.c1oappe.top

split -l 1000 big.log part_
来源：http://hih.svipenyu.cn

[R74] 批量重命名
来源：http://uwz.aizwys.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bep.jqgufenzy.top

[R75] 导出环境变量
来源：http://uhj.tian-w.cn

export PATH="$HOME/bin:$PATH"
来源：http://iwp.dianchejie.cn

[R76] 使用临时文件
来源：http://ncn.pengpengdd.cyou

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lvg.daxiang520.top

[R77] 读取用户输入
来源：http://lxt.jqgufenzy.top

read -rp "请输入: " ans
来源：http://ecv.ctjpmb.com

[R78] 交互式菜单
来源：http://iag.ctjpmb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://xzg.chenjidiqi.icu

[R79] 解析命令行选项
来源：http://nfn.zhengqikj.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wjq.yangfankeji.com

[R80] 查看脚本执行耗时
来源：http://zzq.haohaochexian.top

time ./run.sh
来源：http://xna.cqqwz.cn

================================================================================
来源：http://rzo.wangdashe.top

S. C / C++ 专题
来源：http://eql.yonumen.top

================================================================================
来源：http://zpp.sysykeji.top

[S01] C：Hello World
来源：http://cyu.redwolf501.top

#include <stdio.h>
来源：http://nai.sxryk.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://gvb.yongpay.top

[S02] C：变量与格式化输出
来源：http://gzj.hammf.cn

int a = 10; printf("%d\n", a);
来源：http://ulc.ywan-chungtsiang.top

[S03] C：读入整数
来源：http://zlw.cucudq.cn

int x; scanf("%d", &x);
来源：http://shn.shanyushiyangtech.top

[S04] C：字符串复制
来源：http://vrd.xziqi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://edg.bjfxy.top

[S05] C：字符串长度
来源：http://doc.xuanzx.com

strlen(s)
来源：http://hkp.tian-w.cn

[S06] C：字符串比较
来源：http://dlc.yj202588.top

strcmp(a, b) == 0
来源：http://rfe.bjfxy.top

[S07] C：数组遍历求和
来源：http://uoy.tianlin.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://glc.pycfn.com

[S08] C：动态内存分配与释放
来源：http://zip.pycfn.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wjn.nwbrower.top

[S09] C：结构体定义与初始化
来源：http://day.sxryk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vce.mhx1999.top

[S10] C：指针与解引用
来源：http://xiy.shzxlz.cn

int *p = &a;  *p = 5;
来源：http://bdb.jlsjyb.cn

[S11] C：逐行读文件
来源：http://seo.chenzaomai.com

FILE *f = fopen("a.txt", "r");
来源：http://pvw.hysaishi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ymt.yonumen.top

fclose(f);
来源：http://upj.sxryk.cn

[S12] C：写文件
来源：http://rxy.daria6918.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qfn.kuanghao11.cn

[S13] C：宏定义
来源：http://nqf.jianghu66.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oea.ydzc1.top

[S14] C：枚举
来源：http://jen.fengsongda.top

enum Color { RED, GREEN, BLUE };
来源：http://ftw.xylfe.cn

[S15] C：类型转换
来源：http://tho.andypj.xyz

(double) a / b
来源：http://vfj.jqgfzy.top

[S16] C：位操作置位
来源：http://ohq.dianchejie.cn

x |= (1 << 3);
来源：http://idw.xylfe.cn

[S17] C：安全拼接字符串
来源：http://ncq.pengpengdd.cyou

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bpq.zycfv.cn

[S18] C：命令行参数
来源：http://myc.ydjk.org.cn

int main(int argc, char **argv)
来源：http://dcr.birdmap.top

[S19] C：快速排序
来源：http://agh.fehbvm.com

qsort(a, n, sizeof(int), cmp);
来源：http://bun.guannengcc.top

[S20] C：二分查找
来源：http://gdu.gzhubu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://khu.pycfn.com

[S21] C：字符类别判断
来源：http://vcb.xuanzx.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://dnh.meibo888.top

[S22] C：字符串转数字
来源：http://qul.vqdsnc.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qnr.jqgfzy.top

[S23] C：随机数
来源：http://jhc.zhiwuduotai.top

srand(time(NULL));  int r = rand() % 100;
来源：http://ask.xinyue.icu

[S24] C：获取本地时间
来源：http://bvh.gogol.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fai.daxiang520.top

[S25] C：内存拷贝
来源：http://efq.sweek.top

memcpy(dst, src, n);
来源：http://rbm.snrcjt.cn

[S26] C：内存清零
来源：http://fcl.ehwqpu.com

memset(a, 0, sizeof a);
来源：http://enw.gogol.net.cn

[S27] C：定义常量
来源：http://ulp.hammf.cn

const double PI = 3.14159;
来源：http://twa.sufxvd.cn

[S28] C：静态变量
来源：http://zne.gogol.net.cn

static int counter = 0;
来源：http://yen.jqgfzy.top

[S29] C：变参函数
来源：http://kpr.redwolf501.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://alt.jinghuilouyu.cn

[S30] C：头文件保护
来源：http://hpw.fehbvm.com

#ifndef X_H
来源：http://mpt.hcnkem.com

#define X_H
来源：http://gwi.dianchejie.cn

#endif
来源：http://yoj.yuanzhike.top

[S31] C++：Hello World
来源：http://utu.epnwcf.com

#include <iostream>
来源：http://ctj.svipenyu.cn

int main() { std::cout << "Hello\n"; }
来源：http://fmi.ydzc1.top

[S32] C++：字符串
来源：http://lce.jlsjyb.cn

std::string s = "hi";  s += "!";
来源：http://xat.cqqwz.cn

[S33] C++：vector 增删
来源：http://amy.ydjk.org.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tib.hnqzz.top

[S34] C++：遍历 vector
来源：http://oqo.zhijiandao.cn

for (auto &x : v) { std::cout << x; }
来源：http://toj.haohaochexian.top

[S35] C++：map
来源：http://vlt.chenzaomai.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pbs.shanyushiyangkeji.top

[S36] C++：unordered_map
来源：http://bzu.tarul.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jbu.hongshengwenyu.top

[S37] C++：set
来源：http://uws.yongpay.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rmc.redwolf501.top

[S38] C++：排序
来源：http://cba.yueranfly.top

std::sort(v.begin(), v.end());
来源：http://ueb.havefunace.top

[S39] C++：自定义比较器排序
来源：http://wjz.chenjidiqi.icu

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ose.iojbl.cn

[S40] C++：查找元素
来源：http://yei.shuidangran.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tqm.hcnkem.com

[S41] C++：类与构造函数
来源：http://eyj.shanyushiyangtech.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sva.xuanzx.com

[S42] C++：继承与虚函数
来源：http://dlm.epnwcf.com

class B : public Base { public: void f() override {} };
来源：http://ajc.epnwcf.com

[S43] C++：智能指针
来源：http://sda.yj202588.top

auto p = std::make_unique<int>(5);
来源：http://zlp.birdmap.top

[S44] C++：引用传参
来源：http://fkk.xingfuxueyuan.xyz

void inc(int &x) { ++x; }
来源：http://lks.yfazqb.com

[S45] C++：lambda
来源：http://vzf.zhiwuduotai.top

auto add = [](int a, int b) { return a + b; };
来源：http://xpt.sweek.top

[S46] C++：函数模板
来源：http://abu.cashguo.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://idh.zhijiandao.cn

[S47] C++：结构化绑定遍历
来源：http://wjx.fzhhl.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ncp.daria6918.cn

[S48] C++：逐行读文件
来源：http://sfu.fehbvm.com

std::ifstream in("a.txt");  std::string line;
来源：http://igy.kuanghao11.cn

while (std::getline(in, line)) { }
来源：http://vzt.snrcjt.cn

[S49] C++：写文件
来源：http://vmh.tanke756.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fbg.xziqi.cn

[S50] C++：格式化数字
来源：http://qoj.jiagoushi.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cvi.daxiang520.top

[S51] C++：显式类型转换
来源：http://ayf.pengpengdd.cyou

static_cast<double>(a) / b
来源：http://vlx.sxryk.cn

[S52] C++：const 与 noexcept
来源：http://ylt.yuxming.cn

int size() const noexcept { return n_; }
来源：http://unb.fehbvm.com

[S53] C++：移动语义
来源：http://dkj.xingfuxueyuan.xyz

std::vector<int> w = std::move(v);
来源：http://qka.mhx1999.top

[S54] C++：异常处理
来源：http://pwp.quarkkingdee.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ube.birdmap.top

[S55] C++：结构化绑定
来源：http://mwr.sysykeji.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bfv.shangyingyoupin.top

[S56] C++：optional
来源：http://hyz.yj20258888.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pvs.xingfuxueyuan.xyz

[S57] C++：编译期常量
来源：http://mql.9152youxi.cn

constexpr int N = 10;
来源：http://syx.fktsv.cn

[S58] C++：命名空间
来源：http://kwc.chenlongwang.top

namespace ns { int f() { return 1; } }
来源：http://zzx.xuanzx.com

[S59] C++：静态断言
来源：http://vjc.zhijiandao.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://znk.birdmap.top

[S60] C++：遍历并删除元素
来源：http://hvo.shangyingyoupin.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gdl.fzhhl.top

================================================================================
来源：http://vjj.jiagoushi.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rpo.guowangkeji.top

================================================================================
来源：http://rpe.zycfv.cn

[T01] Kotlin：Hello World
来源：http://pzr.ivvv.top

println("Hello")
来源：http://pga.xziqi.cn

[T02] Kotlin：变量
来源：http://qin.ydjk.org.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qjr.jinqigufen.top

[T03] Kotlin：字符串模板
来源：http://nyb.ppjwa.cn

"值: $b"
来源：http://uni.hfpthk.cn

[T04] Kotlin：空安全
来源：http://lkt.52xcode.cn

val n: String? = null;  n?.length
来源：http://yoy.c1oappe.top

[T05] Kotlin：when 表达式
来源：http://swd.xuetiantiany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ynf.zhixingplan.top

[T06] Kotlin：集合映射
来源：http://oxn.yangfankeji.com

listOf(1, 2, 3).map { it * 2 }
来源：http://wms.bbcook.cn

[T07] Kotlin：集合过滤
来源：http://has.hnqzz.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://nxt.jiagoushi.top

[T08] Kotlin：数据类
来源：http://mma.fehbvm.com

data class User(val name: String, val age: Int)
来源：http://lnm.gogol.net.cn

[T09] Kotlin：扩展函数
来源：http://iwy.vqdsnc.cn

fun String.exclaim() = this + "!"
来源：http://ute.hnxiangtu.top

[T10] Kotlin：默认参数
来源：http://sfh.chenlongwang.top

fun greet(name: String = "World") = "Hi $name"
来源：http://izy.epnwcf.com

[T11] Kotlin：协程
来源：http://ltc.epnwcf.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://rgb.jiagoushi.top

[T12] Kotlin：解构声明
来源：http://qwm.wangshuangyany.cn

val (a, b) = Pair(1, 2)
来源：http://elu.nanxuanxn.top

[T13] Kotlin：只读 Map
来源：http://wfz.zhiwuduotai.top

val m = mapOf("a" to 1)
来源：http://nct.daria6918.cn

[T14] Kotlin：循环
来源：http://nco.hongshengwenyu.top

for (i in 1..10) println(i)
来源：http://hvx.aizwys.cn

[T15] Kotlin：接口
来源：http://mhm.zdbjq.cn

interface Shape { fun area(): Double }
来源：http://aoj.shuidangran.top

[T16] Swift：Hello World
来源：http://ohs.daxiang520.top

print("Hello")
来源：http://hsf.cashguo.top

[T17] Swift：变量与常量
来源：http://ckg.zhijiandao.cn

var a = 1;  let b = 2
来源：http://icz.pengpengdd.cyou

[T18] Swift：字符串插值
来源：http://doh.svipenyu.cn

"值: \(b)"
来源：http://ljg.cqqwz.cn


<!-- 参考信息 -->