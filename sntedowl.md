代发 wailian999

readonly PI=3.14
来源：http://hyg.dashuyun.cn

[R04] 位置参数
来源：http://kaj.xylfe.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xku.chenlongwang.top

[R05] 参数默认值
来源：http://syn.zhijiandao.cn

name="${1:-default}"
来源：http://lmx.yj20258.top

[R06] 判断命令是否存在
来源：http://htp.yj20258.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hrg.gzhubu.top

[R07] if 判断文件
来源：http://seh.jinghuilouyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fsg.tanke756.top

[R08] 数值比较
来源：http://aqy.fktsv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://rij.c1oappe.top

[R09] 字符串比较
来源：http://itv.xuanzx.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pdt.yvedp.cn

[R10] 正则匹配
来源：http://qaj.birdmap.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ydp.shuidangran.top

[R11] case 多分支
来源：http://hul.gzhubu.top

case "$1" in
来源：http://nym.ehwqpu.com

start) echo "启动" ;;
来源：http://blj.xuetiantiany.cn

stop)  echo "停止" ;;
来源：http://cmb.ywan-chungtsiang.top

*)     echo "未知命令" ;;
来源：http://sdo.guannengcc.top

esac
来源：http://mbg.redwolf501.top

[R12] for 遍历文件
来源：http://vlu.jlsjyb.cn

for f in *.txt; do echo "$f"; done
来源：http://wbr.hysaishi.cn

[R13] for 计数循环
来源：http://wpq.chenlongwang.top

for i in {1..10}; do echo "$i"; done
来源：http://scx.chenlongwang.top

[R14] C 风格 for
来源：http://xuq.cucudq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://biu.fzhhl.top

[R15] while 逐行读文件
来源：http://slg.guannengcc.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ehw.dianchejie.cn

[R16] until 等待条件
来源：http://csd.gzhubu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jwn.ehwqpu.com

[R17] 数组定义与取值
来源：http://upm.xuanzx.com

arr=(a b c); echo "${arr[0]}"
来源：http://prp.cdnleiting.top

[R18] 遍历数组
来源：http://hie.jinghuilouyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cqs.xziqi.cn

[R19] 数组长度
来源：http://xkb.yangfankeji.com

echo "${#arr[@]}"
来源：http://twm.yanxiufei.cn

[R20] 关联数组（字典）
来源：http://yhy.sysykeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mqs.mhx1999.top

[R21] 字符串长度
来源：http://wgj.zhijiandao.cn

echo "${#s}"
来源：http://ngv.xziqi.cn

[R22] 截取子串
来源：http://hhl.yuxming.cn

echo "${s:0:5}"
来源：http://ahj.snrcjt.cn

[R23] 字符串替换
来源：http://peu.zhoulong.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ass.zdqjudy.top

[R24] 大小写转换
来源：http://qvu.52xcode.cn

echo "${s^^}"; echo "${s,,}"
来源：http://qcr.xuetiantiany.cn

[R25] 去后缀 / 去前缀
来源：http://xnx.cdnleiting.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://krr.fanxiaobao.xyz

[R26] 命令替换
来源：http://wmf.jiagoushi.top

now=$(date +%F); echo "$now"
来源：http://rit.yj20258.top

[R27] 算术展开
来源：http://yqa.xylfe.cn

echo $((1 + 2 * 3))
来源：http://afk.fanxiaobao.xyz

[R28] 浮点运算
来源：http://iao.ydjk.org.cn

echo "scale=2; 10/3" | bc
来源：http://drj.jyoumei.cn

[R29] 定义函数
来源：http://bbf.hysaishi.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cjq.sxryk.cn

[R30] 函数返回状态码
来源：http://bsu.wangdashe.top

f() { return 0; }; f || echo "失败了"
来源：http://qkq.zycfv.cn

[R31] 局部变量
来源：http://tfh.52xcode.cn

f() { local x=1; echo "$x"; }
来源：http://xgj.gogol.net.cn

[R32] 参数个数校验
来源：http://pzf.snrcjt.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://keq.cqqwz.cn

[R33] 捕获错误并提示行号
来源：http://grx.vehdjk.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wnq.ppjwa.cn

[R34] 退出时清理
来源：http://dhr.wangshuangyany.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qmp.aibaodan.cn

[R35] 后台执行并等待
来源：http://bzu.yongpay.top

sleep 5 & pid=$!; wait "$pid"
来源：http://sco.yangfankeji.com

[R36] 并发执行多个任务
来源：http://suv.zhoulong.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nsi.hcnkem.com

[R37] 把输出赋给变量
来源：http://rvg.gotoacloud.top

files=$(ls -1)
来源：http://jve.chenzaomai.com

[R38] 管道串联
来源：http://ybq.hfpthk.cn

cat a.txt | grep -i error | wc -l
来源：http://okm.quarkkingdee.top

[R39] 重定向标准输出与错误
来源：http://uzk.yj20258.top

cmd > out.log 2>&1
来源：http://wqa.fengsongda.top

[R40] 追加写日志
来源：http://xmo.sjlbkw.cn

echo "log" >> out.log
来源：http://vxb.xuetiantiany.cn

[R41] 丢弃输出
来源：http://oyd.gaohongyu789.top

cmd >/dev/null 2>&1
来源：http://vja.redwolf501.top

[R42] 输入重定向
来源：http://ccp.pycfn.com

wc -l < a.txt
来源：http://hfy.jyoumei.cn

[R43] 按名字查找文件
来源：http://ywb.aibaodan.cn

find . -name "*.log" -type f
来源：http://gyn.wangshuangyany.cn

[R44] 按修改时间查找
来源：http://hki.jinqigufen.top

find . -mtime -7 -type f
来源：http://grg.hesvh.cn

[R45] 批量删除
来源：http://cqx.xinyue.icu

find . -name "*.tmp" -delete
来源：http://ikt.redwolf501.top

[R46] 递归替换文件内容
来源：http://vub.0kj1m.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ywp.yfazqb.com

[R47] sed 单行替换
来源：http://wfp.zycfv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rqe.nanxinkj.top

[R48] awk 取指定列
来源：http://zgx.dashuyun.cn

awk '{print $1, $3}' a.txt
来源：http://xpv.nanxinkj.top

[R49] awk 带条件
来源：http://nuc.xziqi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kbb.shzxlz.cn

[R50] awk 求和
来源：http://ijs.fehbvm.com

awk '{s += $2} END {print s}' a.txt
来源：http://kjh.9152youxi.cn

[R51] 排序去重取前几
来源：http://hyu.sxryk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ujw.dashuyun.cn

[R52] 统计行数
来源：http://hdp.iojbl.cn

wc -l a.txt
来源：http://sky.uphjek.com

[R53] 查看文件头与实时尾
来源：http://use.gotoacloud.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tgc.fzhhl.top

[R54] 比较两个文件
来源：http://sot.dianchejie.cn

diff a.txt b.txt
来源：http://bmy.yfazqb.com

[R55] 压缩与解压
来源：http://uxk.shangyingyoupin.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://otl.zdbjq.cn

[R56] 远程拷贝
来源：http://wmn.mhx1999.top

scp file user@host:/path/
来源：http://trz.hfpthk.cn

[R57] 远程执行命令
来源：http://fal.ppjwa.cn

ssh user@host 'uptime'
来源：http://myo.dashuyun.cn

[R58] 下载文件
来源：http://mzn.sufxvd.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mlq.hongshengwenyu.top

[R59] 发 POST JSON
来源：http://lgn.smart0.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dqm.guannengcc.top

[R60] 只看 HTTP 状态码
来源：http://sfz.jinyuanbaomall.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://uxd.hesvh.cn

[R61] 磁盘占用
来源：http://ttw.chenlongwang.top

df -h;  du -sh *
来源：http://tji.sxryk.cn

[R62] 找最占空间的文件
来源：http://vun.52xcode.cn

du -ah . | sort -rh | head -10
来源：http://svy.havefunace.top

[R63] 内存与进程
来源：http://gtz.pycfn.com

free -h;  ps aux | grep nginx
来源：http://sjc.wangshuangyany.cn

[R64] 结束进程
来源：http://jmv.bbcook.cn

kill -9 $(pgrep -f app.py)
来源：http://nfq.fengsongda.top

[R65] 查看端口占用
来源：http://glg.ppjwa.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://krd.316326.xyz

[R66] 定时任务
来源：http://fui.daria6918.cn

crontab -e;  crontab -l
来源：http://agp.ybcxt.top

[R67] 生成随机十六进制串
来源：http://jct.ydjk.org.cn

openssl rand -hex 16
来源：http://kei.zhongyouzk.top

[R68] 计算文件校验值
来源：http://yul.mhx1999.top

sha256sum a.txt;  md5sum a.txt
来源：http://zfg.hongshengwenyu.top

[R69] 生成随机密码
来源：http://bgn.yvedp.cn

head -c 16 /dev/urandom | base64
来源：http://yts.jqgufenzy.top

[R70] 时间戳与互转
来源：http://xkd.zdqjudy.top

date +%s;  date -d @1700000000
来源：http://rab.yanxiufei.cn

[R71] 日期格式化
来源：http://qju.nanxinkj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vav.jlsjyb.cn

[R72] 等待端口就绪
来源：http://lbd.jianghu66.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ose.ivvv.top

[R73] 分割大日志
来源：http://mll.andypj.xyz

split -l 1000 big.log part_
来源：http://lrs.jianghu66.top

[R74] 批量重命名
来源：http://qpq.zhiwuduotai.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://atl.meibo888.top

[R75] 导出环境变量
来源：http://fwh.hnqzz.top

export PATH="$HOME/bin:$PATH"
来源：http://mpp.fanxiaobao.xyz

[R76] 使用临时文件
来源：http://dyo.shanyushiyangtech.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://esy.xuanzx.com

[R77] 读取用户输入
来源：http://iwq.jianghu66.top

read -rp "请输入: " ans
来源：http://kvw.wangdashe.top

[R78] 交互式菜单
来源：http://pzr.tanke756.top

select opt in a b c; do echo "$opt"; break; done
来源：http://utj.quarkkingdee.top

[R79] 解析命令行选项
来源：http://uub.epnwcf.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ccs.zhengqikj.top

[R80] 查看脚本执行耗时
来源：http://jun.jianghu66.top

time ./run.sh
来源：http://mrc.tian-w.cn

================================================================================
来源：http://lko.andypj.xyz

S. C / C++ 专题
来源：http://ggp.xinyue.icu

================================================================================
来源：http://azd.zhongyouzk.top

[S01] C：Hello World
来源：http://yzp.ydjk.org.cn

#include <stdio.h>
来源：http://yij.fktsv.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://akn.yanxiufei.cn

[S02] C：变量与格式化输出
来源：http://afm.316326.xyz

int a = 10; printf("%d\n", a);
来源：http://yae.xuanzx.com

[S03] C：读入整数
来源：http://idq.xuanzx.com

int x; scanf("%d", &x);
来源：http://wzv.shangyingyoupin.top

[S04] C：字符串复制
来源：http://isd.yj202588.top

char dst[32]; strcpy(dst, "hi");
来源：http://rdt.yuanzhike.top

[S05] C：字符串长度
来源：http://til.52xcode.cn

strlen(s)
来源：http://gym.chenjidiqi.icu

[S06] C：字符串比较
来源：http://ehf.aibaodan.cn

strcmp(a, b) == 0
来源：http://vml.svipenyu.cn

[S07] C：数组遍历求和
来源：http://cgq.redwolf501.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jur.svipenyu.cn

[S08] C：动态内存分配与释放
来源：http://aik.daria6918.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://smo.hongshengwenyu.top

[S09] C：结构体定义与初始化
来源：http://ibb.ppjwa.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://asr.yj20258888.top

[S10] C：指针与解引用
来源：http://xgd.yj20258888.top

int *p = &a;  *p = 5;
来源：http://nbs.gzhubu.top

[S11] C：逐行读文件
来源：http://bmg.jinqigfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://afl.ctjpmb.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://kds.dashuyun.cn

fclose(f);
来源：http://ezd.chenjidiqi.icu

[S12] C：写文件
来源：http://rdc.yfazqb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uty.meibo888.top

[S13] C：宏定义
来源：http://fky.zhijiandao.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://kpg.ppjwa.cn

[S14] C：枚举
来源：http://vca.jianghu66.top

enum Color { RED, GREEN, BLUE };
来源：http://upp.aibaodan.cn

[S15] C：类型转换
来源：http://ycs.guowangkeji.top

(double) a / b
来源：http://cfo.aibaodan.cn

[S16] C：位操作置位
来源：http://fxm.nanxuanxn.top

x |= (1 << 3);
来源：http://vat.nanxuanxn.top

[S17] C：安全拼接字符串
来源：http://svg.zhixingplan.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gzu.meibo888.top

[S18] C：命令行参数
来源：http://lae.sxryk.cn

int main(int argc, char **argv)
来源：http://zbs.wangdashe.top

[S19] C：快速排序
来源：http://uoc.yanxiufei.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cst.yvedp.cn

[S20] C：二分查找
来源：http://neh.bbcook.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bcv.vehdjk.com

[S21] C：字符类别判断
来源：http://yii.yfazqb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://omp.zhengqikj.top

[S22] C：字符串转数字
来源：http://xas.gzhubu.top

atoi("42");  strtod("3.14", NULL);
来源：http://sqz.cqqwz.cn

[S23] C：随机数
来源：http://lka.9152youxi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jxm.shangyingyoupin.top

[S24] C：获取本地时间
来源：http://keh.316326.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://uje.gogol.net.cn

[S25] C：内存拷贝
来源：http://mxf.shangyingyoupin.top

memcpy(dst, src, n);
来源：http://zqd.hysaishi.cn

[S26] C：内存清零
来源：http://laa.hesvh.cn

memset(a, 0, sizeof a);
来源：http://gdy.cqqwz.cn

[S27] C：定义常量
来源：http://pbm.sjlbkw.cn

const double PI = 3.14159;
来源：http://htg.wangshuangyany.cn

[S28] C：静态变量
来源：http://alt.hcnkem.com

static int counter = 0;
来源：http://hdb.nanxuanxn.top

[S29] C：变参函数
来源：http://mbz.sweek.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kgf.shuidangran.top

[S30] C：头文件保护
来源：http://orf.zhixingplan.top

#ifndef X_H
来源：http://ibd.zdqjudy.top

#define X_H
来源：http://fth.shuidangran.top

#endif
来源：http://gwv.tarul.cn

[S31] C++：Hello World
来源：http://kdl.jinqigfzy.top

#include <iostream>
来源：http://rio.shanyushiyangtech.top

int main() { std::cout << "Hello\n"; }
来源：http://zfs.epnwcf.com

[S32] C++：字符串
来源：http://gsu.andypj.xyz

std::string s = "hi";  s += "!";
来源：http://xce.chenlongwang.top

[S33] C++：vector 增删
来源：http://gre.snrcjt.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://elw.mhx1999.top

[S34] C++：遍历 vector
来源：http://wol.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://ikz.sufxvd.cn

[S35] C++：map
来源：http://gjm.xuetiantiany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kyw.dashuyun.cn

[S36] C++：unordered_map
来源：http://irr.xingfuxueyuan.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wws.yj20258.top

[S37] C++：set
来源：http://wse.fanxiaobao.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lyo.svipenyu.cn

[S38] C++：排序
来源：http://mnn.chenlongwang.top

std::sort(v.begin(), v.end());
来源：http://spy.0kj1m.cn

[S39] C++：自定义比较器排序
来源：http://gfc.fzhhl.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tbu.tianlin.xyz

[S40] C++：查找元素
来源：http://dmx.daria6918.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hrf.yanxiufei.cn

[S41] C++：类与构造函数
来源：http://wiq.yj20258.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://enb.tian-w.cn

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com

class B : public Base { public: void f() override {} };
来源：http://fvm.smart0.xyz

[S43] C++：智能指针
来源：http://mhn.ppjwa.cn

auto p = std::make_unique<int>(5);
来源：http://gin.chenjidiqi.icu

[S44] C++：引用传参
来源：http://wkd.hcnkem.com

void inc(int &x) { ++x; }
来源：http://auq.hammf.cn

[S45] C++：lambda
来源：http://fqu.meibo888.top

auto add = [](int a, int b) { return a + b; };
来源：http://fnl.hywenlv.cn

[S46] C++：函数模板
来源：http://yuh.yangfankeji.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dbv.fktsv.cn

[S47] C++：结构化绑定遍历
来源：http://alx.sweek.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://irw.xylfe.cn

[S48] C++：逐行读文件
来源：http://nyh.tianlin.xyz

std::ifstream in("a.txt");  std::string line;
来源：http://rxl.chenlongwang.top

while (std::getline(in, line)) { }
来源：http://opw.chenzaomai.com

[S49] C++：写文件
来源：http://dfj.ybcxt.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ehu.zhixingplan.top

[S50] C++：格式化数字
来源：http://tre.birdmap.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://leb.zhijiandao.cn

[S51] C++：显式类型转换
来源：http://vkk.gotoacloud.top

static_cast<double>(a) / b
来源：http://eyz.snrcjt.cn

[S52] C++：const 与 noexcept
来源：http://ful.mhx1999.top

int size() const noexcept { return n_; }
来源：http://jry.guowangkeji.top

[S53] C++：移动语义
来源：http://xay.zdbjq.cn

std::vector<int> w = std::move(v);
来源：http://aim.jqgufenzy.top

[S54] C++：异常处理
来源：http://rzg.fktsv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ava.chenzaomai.com

[S55] C++：结构化绑定
来源：http://zyb.cdnleiting.top

auto [a, b] = std::make_pair(1, 2);
来源：http://xpf.jinyuanbaomall.cn

[S56] C++：optional
来源：http://abl.zhongyouzk.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vsy.hammf.cn

[S57] C++：编译期常量
来源：http://jzm.zhaomingkeji.xyz

constexpr int N = 10;
来源：http://wzg.meibo888.top

[S58] C++：命名空间
来源：http://ids.yanxiufei.cn

namespace ns { int f() { return 1; } }
来源：http://ovw.guowangkeji.top

[S59] C++：静态断言
来源：http://nze.0kj1m.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jor.zycfv.cn

[S60] C++：遍历并删除元素
来源：http://txn.epnwcf.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zjg.pengpengdd.cyou

================================================================================
来源：http://vzk.pycfn.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://btx.cheryme.top

================================================================================
来源：http://wfw.sjlbkw.cn

[T01] Kotlin：Hello World
来源：http://cfb.ydzc1.top

println("Hello")
来源：http://hfb.andypj.xyz

[T02] Kotlin：变量
来源：http://qgh.ydjk.org.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zui.chenzaomai.com

[T03] Kotlin：字符串模板
来源：http://xuw.dianchejie.cn

"值: $b"
来源：http://sdh.yuxming.cn

[T04] Kotlin：空安全
来源：http://ymb.yanxiufei.cn

val n: String? = null;  n?.length
来源：http://gfd.guannengcc.top


<!-- 参考信息 -->