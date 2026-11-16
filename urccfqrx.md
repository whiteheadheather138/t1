代发 wailian999

name="${1:-default}"
来源：http://isl.shanyushiyangkeji.top

[R06] 判断命令是否存在
来源：http://oxw.jyoumei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lgj.sjlbkw.cn

[R07] if 判断文件
来源：http://goj.cucudq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nqq.havefunace.top

[R08] 数值比较
来源：http://arf.chenzaomai.com

if (( a > b )); then echo "a 更大"; fi
来源：http://xim.chenzaomai.com

[R09] 字符串比较
来源：http://iph.gotoacloud.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qzr.iojbl.cn

[R10] 正则匹配
来源：http://akz.shangyingyoupin.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cqq.gogol.net.cn

[R11] case 多分支
来源：http://axk.dashuyun.cn

case "$1" in
来源：http://odc.sjlbkw.cn

start) echo "启动" ;;
来源：http://hem.nanxinkj.top

stop)  echo "停止" ;;
来源：http://zdo.xinyue.icu

*)     echo "未知命令" ;;
来源：http://qlf.gzhubu.top

esac
来源：http://cks.birdmap.top

[R12] for 遍历文件
来源：http://cke.ywan-chungtsiang.top

for f in *.txt; do echo "$f"; done
来源：http://esi.cqqwz.cn

[R13] for 计数循环
来源：http://pws.shuidangran.top

for i in {1..10}; do echo "$i"; done
来源：http://mga.zhiwuduotai.top

[R14] C 风格 for
来源：http://nsy.xuetiantiany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vrw.daria6918.cn

[R15] while 逐行读文件
来源：http://zfa.hesvh.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wpz.wangdashe.top

[R16] until 等待条件
来源：http://mxq.hnxiangtu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ynf.yueranfly.top

[R17] 数组定义与取值
来源：http://rgr.snrcjt.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vue.jianghu66.top

[R18] 遍历数组
来源：http://qvv.xuetiantiany.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uln.shzxlz.cn

[R19] 数组长度
来源：http://kqs.wangshuangyany.cn

echo "${#arr[@]}"
来源：http://ssi.xziqi.cn

[R20] 关联数组（字典）
来源：http://apq.jyoumei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hxo.jinqigufen.top

[R21] 字符串长度
来源：http://fvm.xuetiantiany.cn

echo "${#s}"
来源：http://zvf.gzhubu.top

[R22] 截取子串
来源：http://jho.ybcxt.top

echo "${s:0:5}"
来源：http://kgd.hfpthk.cn

[R23] 字符串替换
来源：http://bpu.xinyue.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cpg.dianchejie.cn

[R24] 大小写转换
来源：http://icp.feifeiyinyue.top

echo "${s^^}"; echo "${s,,}"
来源：http://ogl.nanxuanxn.top

[R25] 去后缀 / 去前缀
来源：http://wzo.chenlongwang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://oef.havefunace.top

[R26] 命令替换
来源：http://wmj.52xcode.cn

now=$(date +%F); echo "$now"
来源：http://vkp.yanxiufei.cn

[R27] 算术展开
来源：http://laq.ctjpmb.com

echo $((1 + 2 * 3))
来源：http://dyd.ybcxt.top

[R28] 浮点运算
来源：http://oqq.hnxiangtu.top

echo "scale=2; 10/3" | bc
来源：http://fpl.hnxiangtu.top

[R29] 定义函数
来源：http://wwh.jiagoushi.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vfj.yvedp.cn

[R30] 函数返回状态码
来源：http://bmk.jqgufenzy.top

f() { return 0; }; f || echo "失败了"
来源：http://pge.zdbjq.cn

[R31] 局部变量
来源：http://lme.sweek.top

f() { local x=1; echo "$x"; }
来源：http://len.zhoulong.xyz

[R32] 参数个数校验
来源：http://gzt.fengsongda.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lqi.hysaishi.cn

[R33] 捕获错误并提示行号
来源：http://mhv.bjfxy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://fqe.xuetiantiany.cn

[R34] 退出时清理
来源：http://pcg.hfpthk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://vle.dianchejie.cn

[R35] 后台执行并等待
来源：http://kht.shzxlz.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://zcs.zycfv.cn

[R36] 并发执行多个任务
来源：http://wqw.zhixingplan.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cpz.hesvh.cn

[R37] 把输出赋给变量
来源：http://bze.jinqigfzy.top

files=$(ls -1)
来源：http://inv.fktsv.cn

[R38] 管道串联
来源：http://cix.kuanghao11.cn

cat a.txt | grep -i error | wc -l
来源：http://dac.fehbvm.com

[R39] 重定向标准输出与错误
来源：http://yku.chenjidiqi.icu

cmd > out.log 2>&1
来源：http://sav.xingfuxueyuan.xyz

[R40] 追加写日志
来源：http://cor.svipenyu.cn

echo "log" >> out.log
来源：http://pmw.zhoulong.xyz

[R41] 丢弃输出
来源：http://xty.fanxiaobao.xyz

cmd >/dev/null 2>&1
来源：http://eul.jianghu66.top

[R42] 输入重定向
来源：http://hib.yangfankeji.com

wc -l < a.txt
来源：http://jqf.yangfankeji.com

[R43] 按名字查找文件
来源：http://gvn.svipenyu.cn

find . -name "*.log" -type f
来源：http://qrs.ehwqpu.com

[R44] 按修改时间查找
来源：http://njp.uphjek.com

find . -mtime -7 -type f
来源：http://xlu.aizwys.cn

[R45] 批量删除
来源：http://joj.xylfe.cn

find . -name "*.tmp" -delete
来源：http://vgm.cqqwz.cn

[R46] 递归替换文件内容
来源：http://zey.andypj.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://eqz.daria6918.cn

[R47] sed 单行替换
来源：http://avs.yanxiufei.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dhs.pengpengdd.cyou

[R48] awk 取指定列
来源：http://nbg.guannengcc.top

awk '{print $1, $3}' a.txt
来源：http://bbm.hammf.cn

[R49] awk 带条件
来源：http://hty.quarkkingdee.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kfp.fktsv.cn

[R50] awk 求和
来源：http://xbq.pengpengdd.cyou

awk '{s += $2} END {print s}' a.txt
来源：http://awd.xziqi.cn

[R51] 排序去重取前几
来源：http://lbe.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://fep.fzhhl.top

[R52] 统计行数
来源：http://etn.wangdashe.top

wc -l a.txt
来源：http://clh.cqqwz.cn

[R53] 查看文件头与实时尾
来源：http://zmo.hammf.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qsk.yongpay.top

[R54] 比较两个文件
来源：http://jqw.vqdsnc.cn

diff a.txt b.txt
来源：http://eid.yonumen.top

[R55] 压缩与解压
来源：http://ytr.cheryme.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ivu.nwbrower.top

[R56] 远程拷贝
来源：http://wtf.wangdashe.top

scp file user@host:/path/
来源：http://tld.smart0.xyz

[R57] 远程执行命令
来源：http://ski.haohaochexian.top

ssh user@host 'uptime'
来源：http://arv.shangyingyoupin.top

[R58] 下载文件
来源：http://ajs.daria6918.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zuj.birdmap.top

[R59] 发 POST JSON
来源：http://yxc.tanke756.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://knp.vehdjk.com

[R60] 只看 HTTP 状态码
来源：http://tog.guannengcc.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://abx.gogol.net.cn

[R61] 磁盘占用
来源：http://rqr.ybcxt.top

df -h;  du -sh *
来源：http://iva.yueranfly.top

[R62] 找最占空间的文件
来源：http://eac.c1oappe.top

du -ah . | sort -rh | head -10
来源：http://wre.ydzc1.top

[R63] 内存与进程
来源：http://ozc.dashuyun.cn

free -h;  ps aux | grep nginx
来源：http://lap.hywenlv.cn

[R64] 结束进程
来源：http://zkz.uphjek.com

kill -9 $(pgrep -f app.py)
来源：http://htz.yuanzhike.top

[R65] 查看端口占用
来源：http://wsi.jinqigfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ywe.jyoumei.cn

[R66] 定时任务
来源：http://jee.dashuyun.cn

crontab -e;  crontab -l
来源：http://soe.snrcjt.cn

[R67] 生成随机十六进制串
来源：http://nxy.meibo888.top

openssl rand -hex 16
来源：http://lol.guowangkeji.top

[R68] 计算文件校验值
来源：http://rbr.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://ojv.tanke756.top

[R69] 生成随机密码
来源：http://oxv.redwolf501.top

head -c 16 /dev/urandom | base64
来源：http://evl.sufxvd.cn

[R70] 时间戳与互转
来源：http://alc.chenlongwang.top

date +%s;  date -d @1700000000
来源：http://zrs.fehbvm.com

[R71] 日期格式化
来源：http://sqx.quarkkingdee.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://ccm.316326.xyz

[R72] 等待端口就绪
来源：http://hmd.yangfankeji.com

until nc -z localhost 3306; do sleep 1; done
来源：http://rie.birdmap.top

[R73] 分割大日志
来源：http://bdw.aizwys.cn

split -l 1000 big.log part_
来源：http://cei.tarul.cn

[R74] 批量重命名
来源：http://gvi.feifeiyinyue.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cfu.sxryk.cn

[R75] 导出环境变量
来源：http://vhj.snrcjt.cn

export PATH="$HOME/bin:$PATH"
来源：http://exy.316326.xyz

[R76] 使用临时文件
来源：http://qqh.hfpthk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://njr.cheryme.top

[R77] 读取用户输入
来源：http://rqs.nwbrower.top

read -rp "请输入: " ans
来源：http://mlj.daxiang520.top

[R78] 交互式菜单
来源：http://rbc.birdmap.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ajt.hnqzz.top

[R79] 解析命令行选项
来源：http://ado.zhoulong.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://aoq.xinyue.icu

[R80] 查看脚本执行耗时
来源：http://nau.jqgufenzy.top

time ./run.sh
来源：http://twa.tarul.cn

================================================================================
来源：http://lat.yuxming.cn

S. C / C++ 专题
来源：http://rde.sweek.top

================================================================================
来源：http://smz.sufxvd.cn

[S01] C：Hello World
来源：http://sng.jinghuilouyu.cn

#include <stdio.h>
来源：http://lni.pycfn.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://yxj.jinghuilouyu.cn

[S02] C：变量与格式化输出
来源：http://rsn.bjfxy.top

int a = 10; printf("%d\n", a);
来源：http://sgj.aibaodan.cn

[S03] C：读入整数
来源：http://sox.jinyuanbaomall.cn

int x; scanf("%d", &x);
来源：http://hds.daxiang520.top

[S04] C：字符串复制
来源：http://ttx.52xcode.cn

char dst[32]; strcpy(dst, "hi");
来源：http://tsy.tian-w.cn

[S05] C：字符串长度
来源：http://bes.andypj.xyz

strlen(s)
来源：http://frd.xuanzx.com

[S06] C：字符串比较
来源：http://jcj.hesvh.cn

strcmp(a, b) == 0
来源：http://zdu.tianlin.xyz

[S07] C：数组遍历求和
来源：http://efv.yonumen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://trg.fanxiaobao.xyz

[S08] C：动态内存分配与释放
来源：http://nky.chenzaomai.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ayl.fengsongda.top

[S09] C：结构体定义与初始化
来源：http://dsq.xuetiantiany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ujy.hnxiangtu.top

[S10] C：指针与解引用
来源：http://puw.guannengcc.top

int *p = &a;  *p = 5;
来源：http://eyx.jianghu66.top

[S11] C：逐行读文件
来源：http://rqx.cdnleiting.top

FILE *f = fopen("a.txt", "r");
来源：http://rqz.chenlongwang.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://sxf.wangshuangyany.cn

fclose(f);
来源：http://cci.wangshuangyany.cn

[S12] C：写文件
来源：http://cwc.zhiwuduotai.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xey.jianghu66.top

[S13] C：宏定义
来源：http://xyn.xziqi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lsj.havefunace.top

[S14] C：枚举
来源：http://ilp.tian-w.cn

enum Color { RED, GREEN, BLUE };
来源：http://gaz.nwbrower.top

[S15] C：类型转换
来源：http://ows.wangshuangyany.cn

(double) a / b
来源：http://vur.gotoacloud.top

[S16] C：位操作置位
来源：http://imr.pycfn.com

x |= (1 << 3);
来源：http://bhm.yonumen.top

[S17] C：安全拼接字符串
来源：http://jxk.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ior.daria6918.cn

[S18] C：命令行参数
来源：http://xfr.nanxinkj.top

int main(int argc, char **argv)
来源：http://sye.daxiang520.top

[S19] C：快速排序
来源：http://ven.52xcode.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ipk.pycfn.com

[S20] C：二分查找
来源：http://mig.kuanghao11.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://coc.nanxuanxn.top

[S21] C：字符类别判断
来源：http://thz.yj202588.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://amp.yvedp.cn

[S22] C：字符串转数字
来源：http://btw.fzhhl.top

atoi("42");  strtod("3.14", NULL);
来源：http://qvs.shuidangran.top

[S23] C：随机数
来源：http://smq.wangshuangyany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ybr.shangyingyoupin.top

[S24] C：获取本地时间
来源：http://frd.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jmj.zhaomingkeji.xyz

[S25] C：内存拷贝
来源：http://rjy.xinyue.icu

memcpy(dst, src, n);
来源：http://vym.nwbrower.top

[S26] C：内存清零
来源：http://bvk.fktsv.cn

memset(a, 0, sizeof a);
来源：http://jyr.zhengqikj.top

[S27] C：定义常量
来源：http://boj.aizwys.cn

const double PI = 3.14159;
来源：http://mnd.zycfv.cn

[S28] C：静态变量
来源：http://zqv.pycfn.com

static int counter = 0;
来源：http://wwx.ivvv.top

[S29] C：变参函数
来源：http://lrr.nanxuanxn.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lbr.hysaishi.cn

[S30] C：头文件保护
来源：http://huv.tanke756.top

#ifndef X_H
来源：http://roe.tian-w.cn

#define X_H
来源：http://mcx.vqdsnc.cn

#endif
来源：http://vze.hesvh.cn

[S31] C++：Hello World
来源：http://ran.9152youxi.cn

#include <iostream>
来源：http://asb.0kj1m.cn

int main() { std::cout << "Hello\n"; }
来源：http://iob.hongshengwenyu.top

[S32] C++：字符串
来源：http://vuz.wangshuangyany.cn

std::string s = "hi";  s += "!";
来源：http://ves.ydzc1.top

[S33] C++：vector 增删
来源：http://hhz.jianghu66.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dxo.aizwys.cn

[S34] C++：遍历 vector
来源：http://qrv.cdnleiting.top

for (auto &x : v) { std::cout << x; }
来源：http://dvl.xinyue.icu

[S35] C++：map
来源：http://nti.meibo888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hfm.cucudq.cn

[S36] C++：unordered_map
来源：http://lzy.birdmap.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jzt.cashguo.top

[S37] C++：set
来源：http://zdy.hnxiangtu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://aga.jyoumei.cn

[S38] C++：排序
来源：http://lqg.ydzc1.top

std::sort(v.begin(), v.end());
来源：http://equ.zhixingplan.top

[S39] C++：自定义比较器排序
来源：http://ybx.redwolf501.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://fim.guowangkeji.top

[S40] C++：查找元素
来源：http://pyk.yongpay.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gfu.xuetiantiany.cn

[S41] C++：类与构造函数
来源：http://kqi.vehdjk.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ygu.vehdjk.com

[S42] C++：继承与虚函数
来源：http://sja.iojbl.cn

class B : public Base { public: void f() override {} };
来源：http://xfi.c1oappe.top

[S43] C++：智能指针
来源：http://gqz.wangshuangyany.cn

auto p = std::make_unique<int>(5);
来源：http://fsq.xylfe.cn

[S44] C++：引用传参
来源：http://nqa.hysaishi.cn

void inc(int &x) { ++x; }
来源：http://eiu.mhx1999.top

[S45] C++：lambda
来源：http://rvk.vehdjk.com

auto add = [](int a, int b) { return a + b; };
来源：http://ezo.52xcode.cn

[S46] C++：函数模板
来源：http://zah.yj20258.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jcg.xuanzx.com

[S47] C++：结构化绑定遍历
来源：http://tdr.0kj1m.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kjr.zhongyouzk.top

[S48] C++：逐行读文件
来源：http://kbi.tanke756.top

std::ifstream in("a.txt");  std::string line;
来源：http://udm.daria6918.cn

while (std::getline(in, line)) { }
来源：http://roz.epnwcf.com

[S49] C++：写文件
来源：http://bmb.yj202588.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xad.redwolf501.top

[S50] C++：格式化数字
来源：http://nae.ybcxt.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wyz.xziqi.cn

[S51] C++：显式类型转换
来源：http://khj.shuidangran.top

static_cast<double>(a) / b
来源：http://jio.tanke756.top

[S52] C++：const 与 noexcept
来源：http://qzo.cdnleiting.top

int size() const noexcept { return n_; }
来源：http://nkf.zhijiandao.cn

[S53] C++：移动语义
来源：http://zrx.aibaodan.cn

std::vector<int> w = std::move(v);
来源：http://jad.jinqigfzy.top

[S54] C++：异常处理
来源：http://cna.svipenyu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rjo.ivvv.top

[S55] C++：结构化绑定
来源：http://pke.snrcjt.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qaj.wangshuangyany.cn

[S56] C++：optional
来源：http://air.nanxuanxn.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zzl.xuanzx.com

[S57] C++：编译期常量
来源：http://lzy.52xcode.cn

constexpr int N = 10;
来源：http://tqw.fehbvm.com

[S58] C++：命名空间
来源：http://pyc.sxryk.cn

namespace ns { int f() { return 1; } }
来源：http://kjm.jqgufenzy.top

[S59] C++：静态断言
来源：http://zlt.wangshuangyany.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nwt.sysykeji.top

[S60] C++：遍历并删除元素
来源：http://flm.daria6918.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qiy.xinyue.icu

================================================================================
来源：http://cfj.gotoacloud.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://exy.hcnkem.com

================================================================================
来源：http://wbw.smart0.xyz

[T01] Kotlin：Hello World
来源：http://hft.tian-w.cn

println("Hello")
来源：http://uxs.jinghuilouyu.cn

[T02] Kotlin：变量
来源：http://krw.daxiang520.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ycw.hywenlv.cn

[T03] Kotlin：字符串模板
来源：http://vwf.jqgufenzy.top

"值: $b"
来源：http://awy.yuanzhike.top

[T04] Kotlin：空安全
来源：http://wvr.birdmap.top

val n: String? = null;  n?.length
来源：http://kpq.jqgufenzy.top

[T05] Kotlin：when 表达式
来源：http://hsx.fengsongda.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ife.hysaishi.cn

[T06] Kotlin：集合映射
来源：http://syd.vehdjk.com

listOf(1, 2, 3).map { it * 2 }
来源：http://jwi.bjfxy.top


<!-- 参考信息 -->