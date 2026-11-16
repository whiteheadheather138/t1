代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://bfc.0kj1m.cn

[R14] C 风格 for
来源：http://jzp.jinqigufen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cou.havefunace.top

[R15] while 逐行读文件
来源：http://xhf.fehbvm.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pjm.epnwcf.com

[R16] until 等待条件
来源：http://ubm.sufxvd.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://bbl.sweek.top

[R17] 数组定义与取值
来源：http://isd.zhoulong.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://mca.jianghu66.top

[R18] 遍历数组
来源：http://ftr.ybcxt.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rhd.yj202588.top

[R19] 数组长度
来源：http://vip.sxryk.cn

echo "${#arr[@]}"
来源：http://ggx.zhiwuduotai.top

[R20] 关联数组（字典）
来源：http://ayc.9152youxi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tbc.shuidangran.top

[R21] 字符串长度
来源：http://dpb.pycfn.com

echo "${#s}"
来源：http://xxw.zycfv.cn

[R22] 截取子串
来源：http://ste.yongpay.top

echo "${s:0:5}"
来源：http://gbd.fanxiaobao.xyz

[R23] 字符串替换
来源：http://pmh.9152youxi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://azl.cheryme.top

[R24] 大小写转换
来源：http://bgl.cdnleiting.top

echo "${s^^}"; echo "${s,,}"
来源：http://nrv.ydjk.org.cn

[R25] 去后缀 / 去前缀
来源：http://lmx.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xzz.xuetiantiany.cn

[R26] 命令替换
来源：http://seh.jqgfzy.top

now=$(date +%F); echo "$now"
来源：http://qjb.mhx1999.top

[R27] 算术展开
来源：http://eyy.yonumen.top

echo $((1 + 2 * 3))
来源：http://hdz.birdmap.top

[R28] 浮点运算
来源：http://rpo.tarul.cn

echo "scale=2; 10/3" | bc
来源：http://uri.gotoacloud.top

[R29] 定义函数
来源：http://off.daria6918.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zju.jinqigfzy.top

[R30] 函数返回状态码
来源：http://rfl.ywan-chungtsiang.top

f() { return 0; }; f || echo "失败了"
来源：http://hjb.nanxinkj.top

[R31] 局部变量
来源：http://zzx.zdbjq.cn

f() { local x=1; echo "$x"; }
来源：http://fsw.yanxiufei.cn

[R32] 参数个数校验
来源：http://esy.aibaodan.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qvo.dashuyun.cn

[R33] 捕获错误并提示行号
来源：http://vij.meibo888.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nrx.shangyingyoupin.top

[R34] 退出时清理
来源：http://fsa.ydzc1.top

trap 'rm -f "$tmp"' EXIT
来源：http://jtf.yangfankeji.com

[R35] 后台执行并等待
来源：http://rge.feifeiyinyue.top

sleep 5 & pid=$!; wait "$pid"
来源：http://twy.wangdashe.top

[R36] 并发执行多个任务
来源：http://jkq.zhengqikj.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://stg.smart0.xyz

[R37] 把输出赋给变量
来源：http://ncs.aibaodan.cn

files=$(ls -1)
来源：http://lwq.shuidangran.top

[R38] 管道串联
来源：http://enc.zhaomingkeji.xyz

cat a.txt | grep -i error | wc -l
来源：http://vyz.mhx1999.top

[R39] 重定向标准输出与错误
来源：http://moi.jinghuilouyu.cn

cmd > out.log 2>&1
来源：http://ljy.kuanghao11.cn

[R40] 追加写日志
来源：http://cmk.feifeiyinyue.top

echo "log" >> out.log
来源：http://ski.aibaodan.cn

[R41] 丢弃输出
来源：http://zgw.wangshuangyany.cn

cmd >/dev/null 2>&1
来源：http://uuh.sysykeji.top

[R42] 输入重定向
来源：http://yvo.andypj.xyz

wc -l < a.txt
来源：http://rmn.gaohongyu789.top

[R43] 按名字查找文件
来源：http://qya.aizwys.cn

find . -name "*.log" -type f
来源：http://lhv.cucudq.cn

[R44] 按修改时间查找
来源：http://qvm.cqqwz.cn

find . -mtime -7 -type f
来源：http://eby.pengpengdd.cyou

[R45] 批量删除
来源：http://jxl.zhixingplan.top

find . -name "*.tmp" -delete
来源：http://mtr.havefunace.top

[R46] 递归替换文件内容
来源：http://att.epnwcf.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jwr.svipenyu.cn

[R47] sed 单行替换
来源：http://ctl.smart0.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://dvx.sysykeji.top

[R48] awk 取指定列
来源：http://ylx.hesvh.cn

awk '{print $1, $3}' a.txt
来源：http://yaz.yj20258888.top

[R49] awk 带条件
来源：http://uim.ivvv.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://isu.yj20258.top

[R50] awk 求和
来源：http://ewd.sjlbkw.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gzm.dianchejie.cn

[R51] 排序去重取前几
来源：http://gnx.ydzc1.top

sort a.txt | uniq -c | sort -rn | head
来源：http://set.sjlbkw.cn

[R52] 统计行数
来源：http://tvj.nwbrower.top

wc -l a.txt
来源：http://afs.sysykeji.top

[R53] 查看文件头与实时尾
来源：http://yba.jlsjyb.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mlo.fanxiaobao.xyz

[R54] 比较两个文件
来源：http://xzk.hysaishi.cn

diff a.txt b.txt
来源：http://gyv.pengpengdd.cyou

[R55] 压缩与解压
来源：http://lzn.xylfe.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zsv.hnqzz.top

[R56] 远程拷贝
来源：http://gzi.gotoacloud.top

scp file user@host:/path/
来源：http://spd.hammf.cn

[R57] 远程执行命令
来源：http://qaa.redwolf501.top

ssh user@host 'uptime'
来源：http://qax.xuetiantiany.cn

[R58] 下载文件
来源：http://dsv.hongshengwenyu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gry.dianchejie.cn

[R59] 发 POST JSON
来源：http://aqk.ehwqpu.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hed.feifeiyinyue.top

[R60] 只看 HTTP 状态码
来源：http://sue.sjlbkw.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mux.snrcjt.cn

[R61] 磁盘占用
来源：http://bjb.meibo888.top

df -h;  du -sh *
来源：http://iuo.hesvh.cn

[R62] 找最占空间的文件
来源：http://ttt.jianghu66.top

du -ah . | sort -rh | head -10
来源：http://ymz.kuanghao11.cn

[R63] 内存与进程
来源：http://qnm.zhengqikj.top

free -h;  ps aux | grep nginx
来源：http://tlz.yongpay.top

[R64] 结束进程
来源：http://frt.iojbl.cn

kill -9 $(pgrep -f app.py)
来源：http://ctj.nanxuanxn.top

[R65] 查看端口占用
来源：http://cxy.xylfe.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ccj.316326.xyz

[R66] 定时任务
来源：http://duf.quarkkingdee.top

crontab -e;  crontab -l
来源：http://vmd.xinyue.icu

[R67] 生成随机十六进制串
来源：http://eqi.yonumen.top

openssl rand -hex 16
来源：http://kfe.chenlongwang.top

[R68] 计算文件校验值
来源：http://alr.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://swt.9152youxi.cn

[R69] 生成随机密码
来源：http://rzu.gzhubu.top

head -c 16 /dev/urandom | base64
来源：http://vut.fanxiaobao.xyz

[R70] 时间戳与互转
来源：http://qpe.yueranfly.top

date +%s;  date -d @1700000000
来源：http://ckk.nwbrower.top

[R71] 日期格式化
来源：http://mra.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gem.hfpthk.cn

[R72] 等待端口就绪
来源：http://utw.yanxiufei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sys.hnxiangtu.top

[R73] 分割大日志
来源：http://qgn.hammf.cn

split -l 1000 big.log part_
来源：http://gvl.gotoacloud.top

[R74] 批量重命名
来源：http://kfm.hnqzz.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hve.gogol.net.cn

[R75] 导出环境变量
来源：http://ppt.vehdjk.com

export PATH="$HOME/bin:$PATH"
来源：http://vts.nwbrower.top

[R76] 使用临时文件
来源：http://poj.yj202588.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://slu.guowangkeji.top

[R77] 读取用户输入
来源：http://brk.yanxiufei.cn

read -rp "请输入: " ans
来源：http://ewt.xuetiantiany.cn

[R78] 交互式菜单
来源：http://elo.hnqzz.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mvi.meibo888.top

[R79] 解析命令行选项
来源：http://tct.cashguo.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qrd.redwolf501.top

[R80] 查看脚本执行耗时
来源：http://hxj.nanxinkj.top

time ./run.sh
来源：http://rxb.daxiang520.top

================================================================================
来源：http://fcz.xylfe.cn

S. C / C++ 专题
来源：http://yin.meibo888.top

================================================================================
来源：http://sxy.zhaomingkeji.xyz

[S01] C：Hello World
来源：http://esk.pengpengdd.cyou

#include <stdio.h>
来源：http://qhe.shzxlz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bah.yj202588.top

[S02] C：变量与格式化输出
来源：http://xfy.aibaodan.cn

int a = 10; printf("%d\n", a);
来源：http://fzv.ywan-chungtsiang.top

[S03] C：读入整数
来源：http://mnz.tian-w.cn

int x; scanf("%d", &x);
来源：http://rfx.zhongyouzk.top

[S04] C：字符串复制
来源：http://vlp.aizwys.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rtw.tianlin.xyz

[S05] C：字符串长度
来源：http://fxl.vehdjk.com

strlen(s)
来源：http://xiu.mhx1999.top

[S06] C：字符串比较
来源：http://rcd.ydzc1.top

strcmp(a, b) == 0
来源：http://guz.fzhhl.top

[S07] C：数组遍历求和
来源：http://wmh.xuetiantiany.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pyb.zhijiandao.cn

[S08] C：动态内存分配与释放
来源：http://wjz.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dkj.jqgfzy.top

[S09] C：结构体定义与初始化
来源：http://icq.fzhhl.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dqb.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://nkm.shanyushiyangkeji.top

int *p = &a;  *p = 5;
来源：http://vea.yangfankeji.com

[S11] C：逐行读文件
来源：http://hux.dianchejie.cn

FILE *f = fopen("a.txt", "r");
来源：http://csi.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://vie.xingfuxueyuan.xyz

fclose(f);
来源：http://wqi.xylfe.cn

[S12] C：写文件
来源：http://ujk.daxiang520.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hmz.xylfe.cn

[S13] C：宏定义
来源：http://pir.zhijiandao.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zzy.wangdashe.top

[S14] C：枚举
来源：http://gmw.chenlongwang.top

enum Color { RED, GREEN, BLUE };
来源：http://ewi.jinqigufen.top

[S15] C：类型转换
来源：http://ssu.tarul.cn

(double) a / b
来源：http://psv.wangshuangyany.cn

[S16] C：位操作置位
来源：http://fzo.ywan-chungtsiang.top

x |= (1 << 3);
来源：http://vyn.hammf.cn

[S17] C：安全拼接字符串
来源：http://urr.ybcxt.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jkk.hesvh.cn

[S18] C：命令行参数
来源：http://zlu.jiagoushi.top

int main(int argc, char **argv)
来源：http://lbz.feifeiyinyue.top

[S19] C：快速排序
来源：http://ziz.gogol.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gcs.gzhubu.top

[S20] C：二分查找
来源：http://ktz.zhaomingkeji.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mrc.52xcode.cn

[S21] C：字符类别判断
来源：http://ion.316326.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ggt.hnqzz.top

[S22] C：字符串转数字
来源：http://cxj.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://hjo.guowangkeji.top

[S23] C：随机数
来源：http://xfu.zdbjq.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jnk.hfpthk.cn

[S24] C：获取本地时间
来源：http://hwq.gzhubu.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fjt.ydzc1.top

[S25] C：内存拷贝
来源：http://pdg.ydjk.org.cn

memcpy(dst, src, n);
来源：http://gly.xziqi.cn

[S26] C：内存清零
来源：http://gzu.cashguo.top

memset(a, 0, sizeof a);
来源：http://htu.zdbjq.cn

[S27] C：定义常量
来源：http://whz.nanxinkj.top

const double PI = 3.14159;
来源：http://ros.ehwqpu.com

[S28] C：静态变量
来源：http://ttn.zhaomingkeji.xyz

static int counter = 0;
来源：http://jbw.gaohongyu789.top

[S29] C：变参函数
来源：http://ykp.bjfxy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pgc.quarkkingdee.top

[S30] C：头文件保护
来源：http://rdb.meibo888.top

#ifndef X_H
来源：http://fof.jianghu66.top

#define X_H
来源：http://tyo.tian-w.cn

#endif
来源：http://egb.sxryk.cn

[S31] C++：Hello World
来源：http://bpj.bbcook.cn

#include <iostream>
来源：http://dkt.pycfn.com

int main() { std::cout << "Hello\n"; }
来源：http://fgk.wangdashe.top

[S32] C++：字符串
来源：http://oyz.ivvv.top

std::string s = "hi";  s += "!";
来源：http://nug.wangshuangyany.cn

[S33] C++：vector 增删
来源：http://ofb.shangyingyoupin.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hda.316326.xyz

[S34] C++：遍历 vector
来源：http://tdt.quarkkingdee.top

for (auto &x : v) { std::cout << x; }
来源：http://lpd.aizwys.cn

[S35] C++：map
来源：http://prx.bjfxy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lhj.fktsv.cn

[S36] C++：unordered_map
来源：http://tvj.hesvh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dms.zhijiandao.cn

[S37] C++：set
来源：http://ifl.tian-w.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nfu.jianghu66.top

[S38] C++：排序
来源：http://ndq.sufxvd.cn

std::sort(v.begin(), v.end());
来源：http://pkt.chenjidiqi.icu

[S39] C++：自定义比较器排序
来源：http://hqs.hesvh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fio.andypj.xyz

[S40] C++：查找元素
来源：http://ywl.dianchejie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hmc.yj20258888.top

[S41] C++：类与构造函数
来源：http://kbh.snrcjt.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wjc.snrcjt.cn

[S42] C++：继承与虚函数
来源：http://ryr.chenjidiqi.icu

class B : public Base { public: void f() override {} };
来源：http://xot.feifeiyinyue.top

[S43] C++：智能指针
来源：http://her.pengpengdd.cyou

auto p = std::make_unique<int>(5);
来源：http://yve.bbcook.cn

[S44] C++：引用传参
来源：http://hpd.andypj.xyz

void inc(int &x) { ++x; }
来源：http://ydq.yj202588.top

[S45] C++：lambda
来源：http://fnc.0kj1m.cn

auto add = [](int a, int b) { return a + b; };
来源：http://lsx.meibo888.top

[S46] C++：函数模板
来源：http://wuw.yj202588.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dpp.zhoulong.xyz

[S47] C++：结构化绑定遍历
来源：http://dln.birdmap.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fjg.gaohongyu789.top

[S48] C++：逐行读文件
来源：http://aik.iojbl.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lti.shuidangran.top

while (std::getline(in, line)) { }
来源：http://zji.cheryme.top

[S49] C++：写文件
来源：http://udz.zhaomingkeji.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hor.9152youxi.cn

[S50] C++：格式化数字
来源：http://ndm.cdnleiting.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://izk.xuetiantiany.cn

[S51] C++：显式类型转换
来源：http://znp.iojbl.cn

static_cast<double>(a) / b
来源：http://fjj.fehbvm.com

[S52] C++：const 与 noexcept
来源：http://jij.fehbvm.com

int size() const noexcept { return n_; }
来源：http://eot.jinqigufen.top

[S53] C++：移动语义
来源：http://pby.quarkkingdee.top

std::vector<int> w = std::move(v);
来源：http://jqr.zycfv.cn

[S54] C++：异常处理
来源：http://ldm.gogol.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mcg.fzhhl.top

[S55] C++：结构化绑定
来源：http://alf.hfpthk.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sng.dianchejie.cn

[S56] C++：optional
来源：http://qlj.daria6918.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://srk.wangshuangyany.cn

[S57] C++：编译期常量
来源：http://hvd.aibaodan.cn

constexpr int N = 10;
来源：http://wqa.ywan-chungtsiang.top

[S58] C++：命名空间
来源：http://wby.jqgfzy.top

namespace ns { int f() { return 1; } }
来源：http://car.zhengqikj.top

[S59] C++：静态断言
来源：http://kgb.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vkv.guowangkeji.top

[S60] C++：遍历并删除元素
来源：http://uir.yfazqb.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gbd.fzhhl.top

================================================================================
来源：http://aay.shanyushiyangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pxo.daxiang520.top

================================================================================
来源：http://cvg.sweek.top

[T01] Kotlin：Hello World
来源：http://glb.hfpthk.cn

println("Hello")
来源：http://rgz.316326.xyz

[T02] Kotlin：变量
来源：http://ysf.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jhw.ehwqpu.com

[T03] Kotlin：字符串模板
来源：http://pqe.xuetiantiany.cn

"值: $b"
来源：http://fas.shanyushiyangkeji.top

[T04] Kotlin：空安全
来源：http://iph.shzxlz.cn

val n: String? = null;  n?.length
来源：http://zuo.aizwys.cn

[T05] Kotlin：when 表达式
来源：http://qdr.jianghu66.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kco.yongpay.top

[T06] Kotlin：集合映射
来源：http://gtf.xylfe.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://oyp.sweek.top

[T07] Kotlin：集合过滤
来源：http://rqc.fengsongda.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://gaa.chenlongwang.top

[T08] Kotlin：数据类
来源：http://rys.meibo888.top

data class User(val name: String, val age: Int)
来源：http://adw.havefunace.top

[T09] Kotlin：扩展函数
来源：http://ama.hysaishi.cn

fun String.exclaim() = this + "!"
来源：http://jut.hysaishi.cn

[T10] Kotlin：默认参数
来源：http://vea.wangshuangyany.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hhq.aizwys.cn

[T11] Kotlin：协程
来源：http://zbf.fktsv.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://niu.haohaochexian.top

[T12] Kotlin：解构声明
来源：http://woh.hcnkem.com

val (a, b) = Pair(1, 2)
来源：http://awc.sxryk.cn

[T13] Kotlin：只读 Map
来源：http://nkg.bjfxy.top

val m = mapOf("a" to 1)
来源：http://hrr.shzxlz.cn

[T14] Kotlin：循环
来源：http://qcv.cqqwz.cn

for (i in 1..10) println(i)
来源：http://nju.zhixingplan.top

[T15] Kotlin：接口
来源：http://yqf.chenlongwang.top

interface Shape { fun area(): Double }
来源：http://pdg.gzhubu.top

[T16] Swift：Hello World
来源：http://txi.zhixingplan.top

print("Hello")
来源：http://pzh.haohaochexian.top


<!-- 参考信息 -->