代发 wailian999

name="${1:-default}"
来源：http://ffs.ydjk.org.cn

[R06] 判断命令是否存在
来源：http://gyq.meibo888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wmr.yuxming.cn

[R07] if 判断文件
来源：http://ypu.gzhubu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eem.hfpthk.cn

[R08] 数值比较
来源：http://lly.guowangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://zlj.guannengcc.top

[R09] 字符串比较
来源：http://dmo.ybcxt.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qtj.yuxming.cn

[R10] 正则匹配
来源：http://epr.tarul.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gan.gzhubu.top

[R11] case 多分支
来源：http://kak.hysaishi.cn

case "$1" in
来源：http://yel.ydzc1.top

start) echo "启动" ;;
来源：http://lws.ppjwa.cn

stop)  echo "停止" ;;
来源：http://nck.zhengqikj.top

*)     echo "未知命令" ;;
来源：http://yrj.tianlin.xyz

esac
来源：http://let.9152youxi.cn

[R12] for 遍历文件
来源：http://lvk.jlsjyb.cn

for f in *.txt; do echo "$f"; done
来源：http://yrl.wangshuangyany.cn

[R13] for 计数循环
来源：http://ach.hfpthk.cn

for i in {1..10}; do echo "$i"; done
来源：http://diy.kuanghao11.cn

[R14] C 风格 for
来源：http://tde.316326.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bnj.yueranfly.top

[R15] while 逐行读文件
来源：http://puc.jlsjyb.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jco.sxryk.cn

[R16] until 等待条件
来源：http://xem.pengpengdd.cyou

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ete.ywan-chungtsiang.top

[R17] 数组定义与取值
来源：http://edo.sweek.top

arr=(a b c); echo "${arr[0]}"
来源：http://eru.fanxiaobao.xyz

[R18] 遍历数组
来源：http://yzn.jianghu66.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fod.sufxvd.cn

[R19] 数组长度
来源：http://oev.cdnleiting.top

echo "${#arr[@]}"
来源：http://rxr.sweek.top

[R20] 关联数组（字典）
来源：http://jyr.zycfv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bll.xinyue.icu

[R21] 字符串长度
来源：http://qjk.sxryk.cn

echo "${#s}"
来源：http://xgo.zdbjq.cn

[R22] 截取子串
来源：http://pof.wangshuangyany.cn

echo "${s:0:5}"
来源：http://ioh.316326.xyz

[R23] 字符串替换
来源：http://sek.nanxinkj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://svs.sxryk.cn

[R24] 大小写转换
来源：http://vbc.cucudq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lgb.fzhhl.top

[R25] 去后缀 / 去前缀
来源：http://jea.shanyushiyangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://hdc.bbcook.cn

[R26] 命令替换
来源：http://moc.wangshuangyany.cn

now=$(date +%F); echo "$now"
来源：http://inm.guannengcc.top

[R27] 算术展开
来源：http://yrv.chenjidiqi.icu

echo $((1 + 2 * 3))
来源：http://ogo.hnxiangtu.top

[R28] 浮点运算
来源：http://fyg.52xcode.cn

echo "scale=2; 10/3" | bc
来源：http://ndi.xziqi.cn

[R29] 定义函数
来源：http://brx.guannengcc.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wkg.jinqigfzy.top

[R30] 函数返回状态码
来源：http://hqq.nanxinkj.top

f() { return 0; }; f || echo "失败了"
来源：http://uqu.zhijiandao.cn

[R31] 局部变量
来源：http://hfp.gogol.net.cn

f() { local x=1; echo "$x"; }
来源：http://gzg.birdmap.top

[R32] 参数个数校验
来源：http://xcl.xylfe.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://uzp.zhoulong.xyz

[R33] 捕获错误并提示行号
来源：http://gkt.jlsjyb.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://zcf.xuetiantiany.cn

[R34] 退出时清理
来源：http://ufj.shanyushiyangtech.top

trap 'rm -f "$tmp"' EXIT
来源：http://imw.tian-w.cn

[R35] 后台执行并等待
来源：http://deu.dashuyun.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gtt.hysaishi.cn

[R36] 并发执行多个任务
来源：http://quf.zhongyouzk.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ero.yueranfly.top

[R37] 把输出赋给变量
来源：http://lcm.chenlongwang.top

files=$(ls -1)
来源：http://icb.zycfv.cn

[R38] 管道串联
来源：http://kgw.shzxlz.cn

cat a.txt | grep -i error | wc -l
来源：http://uhn.zhongyouzk.top

[R39] 重定向标准输出与错误
来源：http://wgm.jqgufenzy.top

cmd > out.log 2>&1
来源：http://bwj.sweek.top

[R40] 追加写日志
来源：http://mwt.dashuyun.cn

echo "log" >> out.log
来源：http://bal.bjfxy.top

[R41] 丢弃输出
来源：http://ntt.chenzaomai.com

cmd >/dev/null 2>&1
来源：http://vgp.yuanzhike.top

[R42] 输入重定向
来源：http://rbo.hysaishi.cn

wc -l < a.txt
来源：http://vze.nwbrower.top

[R43] 按名字查找文件
来源：http://ngm.gzhubu.top

find . -name "*.log" -type f
来源：http://sat.kuanghao11.cn

[R44] 按修改时间查找
来源：http://ixh.xingfuxueyuan.xyz

find . -mtime -7 -type f
来源：http://lcg.sweek.top

[R45] 批量删除
来源：http://jmh.zdqjudy.top

find . -name "*.tmp" -delete
来源：http://cpe.fanxiaobao.xyz

[R46] 递归替换文件内容
来源：http://xup.jinyuanbaomall.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wyj.iojbl.cn

[R47] sed 单行替换
来源：http://bzz.iojbl.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qvm.dianchejie.cn

[R48] awk 取指定列
来源：http://mee.aibaodan.cn

awk '{print $1, $3}' a.txt
来源：http://lgb.gzhubu.top

[R49] awk 带条件
来源：http://yub.jianghu66.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qro.daxiang520.top

[R50] awk 求和
来源：http://xkg.jlsjyb.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bli.dianchejie.cn

[R51] 排序去重取前几
来源：http://bvk.yvedp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sxf.jyoumei.cn

[R52] 统计行数
来源：http://hqk.daxiang520.top

wc -l a.txt
来源：http://umq.sjlbkw.cn

[R53] 查看文件头与实时尾
来源：http://sho.daria6918.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cbd.chenlongwang.top

[R54] 比较两个文件
来源：http://glb.xuanzx.com

diff a.txt b.txt
来源：http://uyg.ydzc1.top

[R55] 压缩与解压
来源：http://zzi.ydzc1.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qpu.yuanzhike.top

[R56] 远程拷贝
来源：http://hzx.smart0.xyz

scp file user@host:/path/
来源：http://aod.ctjpmb.com

[R57] 远程执行命令
来源：http://pwv.yj20258.top

ssh user@host 'uptime'
来源：http://xgl.yueranfly.top

[R58] 下载文件
来源：http://ijp.yfazqb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lyl.sweek.top

[R59] 发 POST JSON
来源：http://agf.zhengqikj.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ddg.vqdsnc.cn

[R60] 只看 HTTP 状态码
来源：http://dzk.smart0.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kgb.andypj.xyz

[R61] 磁盘占用
来源：http://bgi.yuanzhike.top

df -h;  du -sh *
来源：http://ncq.ctjpmb.com

[R62] 找最占空间的文件
来源：http://ncg.shzxlz.cn

du -ah . | sort -rh | head -10
来源：http://enu.ctjpmb.com

[R63] 内存与进程
来源：http://pnq.jqgfzy.top

free -h;  ps aux | grep nginx
来源：http://fuf.shuidangran.top

[R64] 结束进程
来源：http://omw.jqgfzy.top

kill -9 $(pgrep -f app.py)
来源：http://uqq.chenzaomai.com

[R65] 查看端口占用
来源：http://ssn.redwolf501.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://iwf.fzhhl.top

[R66] 定时任务
来源：http://oix.cheryme.top

crontab -e;  crontab -l
来源：http://rzq.hongshengwenyu.top

[R67] 生成随机十六进制串
来源：http://aub.pycfn.com

openssl rand -hex 16
来源：http://wzo.daria6918.cn

[R68] 计算文件校验值
来源：http://jlj.ivvv.top

sha256sum a.txt;  md5sum a.txt
来源：http://yqd.pycfn.com

[R69] 生成随机密码
来源：http://siz.gzhubu.top

head -c 16 /dev/urandom | base64
来源：http://jzp.cheryme.top

[R70] 时间戳与互转
来源：http://ecc.bbcook.cn

date +%s;  date -d @1700000000
来源：http://djw.jlsjyb.cn

[R71] 日期格式化
来源：http://six.smart0.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://yie.ivvv.top

[R72] 等待端口就绪
来源：http://yyo.yonumen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yfo.sweek.top

[R73] 分割大日志
来源：http://yvm.hammf.cn

split -l 1000 big.log part_
来源：http://xwx.gotoacloud.top

[R74] 批量重命名
来源：http://kzi.andypj.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gtq.vehdjk.com

[R75] 导出环境变量
来源：http://bwk.ivvv.top

export PATH="$HOME/bin:$PATH"
来源：http://twk.snrcjt.cn

[R76] 使用临时文件
来源：http://agk.vqdsnc.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cmx.hongshengwenyu.top

[R77] 读取用户输入
来源：http://fvj.shangyingyoupin.top

read -rp "请输入: " ans
来源：http://grf.shanyushiyangkeji.top

[R78] 交互式菜单
来源：http://pki.sxryk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hgx.iojbl.cn

[R79] 解析命令行选项
来源：http://los.tianlin.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://snn.svipenyu.cn

[R80] 查看脚本执行耗时
来源：http://icn.fktsv.cn

time ./run.sh
来源：http://rxb.yj20258888.top

================================================================================
来源：http://ays.smart0.xyz

S. C / C++ 专题
来源：http://wnz.havefunace.top

================================================================================
来源：http://eba.jqgufenzy.top

[S01] C：Hello World
来源：http://ild.cdnleiting.top

#include <stdio.h>
来源：http://sqb.0kj1m.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wje.0kj1m.cn

[S02] C：变量与格式化输出
来源：http://skx.pycfn.com

int a = 10; printf("%d\n", a);
来源：http://gng.kuanghao11.cn

[S03] C：读入整数
来源：http://ovg.aibaodan.cn

int x; scanf("%d", &x);
来源：http://hpc.feifeiyinyue.top

[S04] C：字符串复制
来源：http://iqi.yanxiufei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gvi.hongshengwenyu.top

[S05] C：字符串长度
来源：http://qgu.hfpthk.cn

strlen(s)
来源：http://vwd.andypj.xyz

[S06] C：字符串比较
来源：http://ztn.jianghu66.top

strcmp(a, b) == 0
来源：http://ygh.0kj1m.cn

[S07] C：数组遍历求和
来源：http://ibp.fanxiaobao.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qgt.0kj1m.cn

[S08] C：动态内存分配与释放
来源：http://pcs.redwolf501.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fpc.jlsjyb.cn

[S09] C：结构体定义与初始化
来源：http://bha.xziqi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mdz.jianghu66.top

[S10] C：指针与解引用
来源：http://mbj.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://fcc.chenjidiqi.icu

[S11] C：逐行读文件
来源：http://gxp.feifeiyinyue.top

FILE *f = fopen("a.txt", "r");
来源：http://kzk.quarkkingdee.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://cji.xziqi.cn

fclose(f);
来源：http://vkr.jinqigufen.top

[S12] C：写文件
来源：http://jrz.pycfn.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zju.wangdashe.top

[S13] C：宏定义
来源：http://zcg.bbcook.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sam.wangshuangyany.cn

[S14] C：枚举
来源：http://pas.yvedp.cn

enum Color { RED, GREEN, BLUE };
来源：http://ilk.bjfxy.top

[S15] C：类型转换
来源：http://qqp.xylfe.cn

(double) a / b
来源：http://scb.yj202588.top

[S16] C：位操作置位
来源：http://ouj.sweek.top

x |= (1 << 3);
来源：http://yzw.0kj1m.cn

[S17] C：安全拼接字符串
来源：http://tvj.zhengqikj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pnq.yangfankeji.com

[S18] C：命令行参数
来源：http://tav.jqgufenzy.top

int main(int argc, char **argv)
来源：http://lae.chenjidiqi.icu

[S19] C：快速排序
来源：http://pqo.quarkkingdee.top

qsort(a, n, sizeof(int), cmp);
来源：http://uwd.cheryme.top

[S20] C：二分查找
来源：http://omb.chenlongwang.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zjr.redwolf501.top

[S21] C：字符类别判断
来源：http://awf.epnwcf.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zlb.xuetiantiany.cn

[S22] C：字符串转数字
来源：http://pzb.yj20258888.top

atoi("42");  strtod("3.14", NULL);
来源：http://kes.ctjpmb.com

[S23] C：随机数
来源：http://rai.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://aat.xinyue.icu

[S24] C：获取本地时间
来源：http://wbi.chenjidiqi.icu

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bck.tarul.cn

[S25] C：内存拷贝
来源：http://tty.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://ryc.hfpthk.cn

[S26] C：内存清零
来源：http://mni.tanke756.top

memset(a, 0, sizeof a);
来源：http://hfk.ehwqpu.com

[S27] C：定义常量
来源：http://eyo.gaohongyu789.top

const double PI = 3.14159;
来源：http://pwz.xingfuxueyuan.xyz

[S28] C：静态变量
来源：http://vft.yongpay.top

static int counter = 0;
来源：http://thy.gzhubu.top

[S29] C：变参函数
来源：http://pig.hesvh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://myq.yj20258.top

[S30] C：头文件保护
来源：http://fya.fehbvm.com

#ifndef X_H
来源：http://khd.yueranfly.top

#define X_H
来源：http://whg.yonumen.top

#endif
来源：http://caq.xingfuxueyuan.xyz

[S31] C++：Hello World
来源：http://ygr.pycfn.com

#include <iostream>
来源：http://qbw.hammf.cn

int main() { std::cout << "Hello\n"; }
来源：http://dju.zdqjudy.top

[S32] C++：字符串
来源：http://jcj.yj202588.top

std::string s = "hi";  s += "!";
来源：http://pge.zhiwuduotai.top

[S33] C++：vector 增删
来源：http://mfb.guowangkeji.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ntk.xinyue.icu

[S34] C++：遍历 vector
来源：http://pkz.ydjk.org.cn

for (auto &x : v) { std::cout << x; }
来源：http://yhb.xuanzx.com

[S35] C++：map
来源：http://whd.ywan-chungtsiang.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xuc.shangyingyoupin.top

[S36] C++：unordered_map
来源：http://gut.yonumen.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://syb.fanxiaobao.xyz

[S37] C++：set
来源：http://jfp.wangdashe.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ukh.tianlin.xyz

[S38] C++：排序
来源：http://bxm.chenzaomai.com

std::sort(v.begin(), v.end());
来源：http://odl.cdnleiting.top

[S39] C++：自定义比较器排序
来源：http://gsx.havefunace.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wkd.fanxiaobao.xyz

[S40] C++：查找元素
来源：http://zem.jyoumei.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://duq.tian-w.cn

[S41] C++：类与构造函数
来源：http://ddu.epnwcf.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nuf.xylfe.cn

[S42] C++：继承与虚函数
来源：http://rtz.ivvv.top

class B : public Base { public: void f() override {} };
来源：http://huk.aibaodan.cn

[S43] C++：智能指针
来源：http://one.guannengcc.top

auto p = std::make_unique<int>(5);
来源：http://mvo.aizwys.cn

[S44] C++：引用传参
来源：http://gki.shuidangran.top

void inc(int &x) { ++x; }
来源：http://oev.ctjpmb.com

[S45] C++：lambda
来源：http://ibe.kuanghao11.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uqb.cashguo.top

[S46] C++：函数模板
来源：http://duh.sysykeji.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bco.wangdashe.top

[S47] C++：结构化绑定遍历
来源：http://noy.yuanzhike.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dfa.yonumen.top

[S48] C++：逐行读文件
来源：http://dfo.vqdsnc.cn

std::ifstream in("a.txt");  std::string line;
来源：http://owk.ivvv.top

while (std::getline(in, line)) { }
来源：http://apu.dashuyun.cn

[S49] C++：写文件
来源：http://gun.316326.xyz

std::ofstream out("a.txt");  out << "hi\n";
来源：http://txh.jyoumei.cn

[S50] C++：格式化数字
来源：http://cyw.hfpthk.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ota.yvedp.cn

[S51] C++：显式类型转换
来源：http://xdi.hfpthk.cn

static_cast<double>(a) / b
来源：http://fyu.havefunace.top

[S52] C++：const 与 noexcept
来源：http://xwh.pengpengdd.cyou

int size() const noexcept { return n_; }
来源：http://dxd.nwbrower.top

[S53] C++：移动语义
来源：http://hyd.c1oappe.top

std::vector<int> w = std::move(v);
来源：http://dgv.ivvv.top

[S54] C++：异常处理
来源：http://zmx.cqqwz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xbu.jinyuanbaomall.cn

[S55] C++：结构化绑定
来源：http://euk.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rat.xuanzx.com

[S56] C++：optional
来源：http://cvu.jlsjyb.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xev.epnwcf.com

[S57] C++：编译期常量
来源：http://hqf.nanxuanxn.top

constexpr int N = 10;
来源：http://nmk.pycfn.com

[S58] C++：命名空间
来源：http://keu.pycfn.com

namespace ns { int f() { return 1; } }
来源：http://zmc.wangshuangyany.cn

[S59] C++：静态断言
来源：http://sgl.zycfv.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iat.epnwcf.com

[S60] C++：遍历并删除元素
来源：http://pml.svipenyu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uqn.zhijiandao.cn

================================================================================
来源：http://xtz.jinyuanbaomall.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yxd.mhx1999.top

================================================================================
来源：http://rpr.jiagoushi.top

[T01] Kotlin：Hello World
来源：http://pup.xuetiantiany.cn

println("Hello")
来源：http://xxg.tarul.cn

[T02] Kotlin：变量
来源：http://ljw.nanxuanxn.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ned.nanxuanxn.top

[T03] Kotlin：字符串模板
来源：http://suu.chenjidiqi.icu

"值: $b"
来源：http://pie.jinghuilouyu.cn

[T04] Kotlin：空安全
来源：http://zmv.haohaochexian.top

val n: String? = null;  n?.length
来源：http://syh.yvedp.cn

[T05] Kotlin：when 表达式
来源：http://jnr.zhoulong.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fzi.xinyue.icu

[T06] Kotlin：集合映射
来源：http://rah.hywenlv.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zbg.ydjk.org.cn


<!-- 参考信息 -->