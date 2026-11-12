代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tgw.9152youxi.cn

[R10] 正则匹配
来源：http://fyp.ydjk.org.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ute.yueranfly.top

[R11] case 多分支
来源：http://ibo.zhaomingkeji.xyz

case "$1" in
来源：http://njl.quarkkingdee.top

start) echo "启动" ;;
来源：http://swh.yanxiufei.cn

stop)  echo "停止" ;;
来源：http://dhz.zhongyouzk.top

*)     echo "未知命令" ;;
来源：http://ebg.sysykeji.top

esac
来源：http://mrk.pycfn.com

[R12] for 遍历文件
来源：http://gmj.epnwcf.com

for f in *.txt; do echo "$f"; done
来源：http://jiz.9152youxi.cn

[R13] for 计数循环
来源：http://btv.yfazqb.com

for i in {1..10}; do echo "$i"; done
来源：http://zud.jqgfzy.top

[R14] C 风格 for
来源：http://onp.vqdsnc.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rdu.shzxlz.cn

[R15] while 逐行读文件
来源：http://myt.chenlongwang.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mls.bbcook.cn

[R16] until 等待条件
来源：http://dli.52xcode.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jfm.fengsongda.top

[R17] 数组定义与取值
来源：http://gfr.chenzaomai.com

arr=(a b c); echo "${arr[0]}"
来源：http://nry.zhixingplan.top

[R18] 遍历数组
来源：http://rcx.316326.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lhr.pengpengdd.cyou

[R19] 数组长度
来源：http://atp.dashuyun.cn

echo "${#arr[@]}"
来源：http://aez.yuxming.cn

[R20] 关联数组（字典）
来源：http://uks.haohaochexian.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://joe.hysaishi.cn

[R21] 字符串长度
来源：http://zfg.hnxiangtu.top

echo "${#s}"
来源：http://fft.meibo888.top

[R22] 截取子串
来源：http://aic.ydzc1.top

echo "${s:0:5}"
来源：http://dty.xuanzx.com

[R23] 字符串替换
来源：http://cqe.hysaishi.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vdi.svipenyu.cn

[R24] 大小写转换
来源：http://yuy.gzhubu.top

echo "${s^^}"; echo "${s,,}"
来源：http://wek.shanyushiyangkeji.top

[R25] 去后缀 / 去前缀
来源：http://stm.yangfankeji.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://gua.vqdsnc.cn

[R26] 命令替换
来源：http://eec.cucudq.cn

now=$(date +%F); echo "$now"
来源：http://kwv.daria6918.cn

[R27] 算术展开
来源：http://tiv.snrcjt.cn

echo $((1 + 2 * 3))
来源：http://nph.nanxinkj.top

[R28] 浮点运算
来源：http://yvg.tian-w.cn

echo "scale=2; 10/3" | bc
来源：http://fwd.cqqwz.cn

[R29] 定义函数
来源：http://cgt.tianlin.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ufq.tianlin.xyz

[R30] 函数返回状态码
来源：http://pxl.hammf.cn

f() { return 0; }; f || echo "失败了"
来源：http://gli.xinyue.icu

[R31] 局部变量
来源：http://mln.yuanzhike.top

f() { local x=1; echo "$x"; }
来源：http://gyv.sysykeji.top

[R32] 参数个数校验
来源：http://rja.vehdjk.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ucg.ydjk.org.cn

[R33] 捕获错误并提示行号
来源：http://qsx.snrcjt.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://veb.guowangkeji.top

[R34] 退出时清理
来源：http://aag.cashguo.top

trap 'rm -f "$tmp"' EXIT
来源：http://xjl.zdbjq.cn

[R35] 后台执行并等待
来源：http://qjd.zycfv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://rrb.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://aei.c1oappe.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://yws.zdqjudy.top

[R37] 把输出赋给变量
来源：http://kfz.feifeiyinyue.top

files=$(ls -1)
来源：http://abf.nanxuanxn.top

[R38] 管道串联
来源：http://mlf.c1oappe.top

cat a.txt | grep -i error | wc -l
来源：http://oto.dashuyun.cn

[R39] 重定向标准输出与错误
来源：http://dnz.jyoumei.cn

cmd > out.log 2>&1
来源：http://dsk.jqgufenzy.top

[R40] 追加写日志
来源：http://mtp.hesvh.cn

echo "log" >> out.log
来源：http://gqs.ywan-chungtsiang.top

[R41] 丢弃输出
来源：http://ima.cqqwz.cn

cmd >/dev/null 2>&1
来源：http://umn.xingfuxueyuan.xyz

[R42] 输入重定向
来源：http://bmd.xuanzx.com

wc -l < a.txt
来源：http://hci.guannengcc.top

[R43] 按名字查找文件
来源：http://rvm.316326.xyz

find . -name "*.log" -type f
来源：http://xzq.yvedp.cn

[R44] 按修改时间查找
来源：http://uxf.ppjwa.cn

find . -mtime -7 -type f
来源：http://jtk.quarkkingdee.top

[R45] 批量删除
来源：http://yzg.sxryk.cn

find . -name "*.tmp" -delete
来源：http://uhj.xziqi.cn

[R46] 递归替换文件内容
来源：http://xlu.shuidangran.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://aku.shanyushiyangtech.top

[R47] sed 单行替换
来源：http://sws.zdqjudy.top

sed -i 's/foo/bar/g' a.txt
来源：http://tsb.tarul.cn

[R48] awk 取指定列
来源：http://wgq.tian-w.cn

awk '{print $1, $3}' a.txt
来源：http://rov.hammf.cn

[R49] awk 带条件
来源：http://kei.chenjidiqi.icu

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ijh.ydjk.org.cn

[R50] awk 求和
来源：http://wsx.yueranfly.top

awk '{s += $2} END {print s}' a.txt
来源：http://lhl.cucudq.cn

[R51] 排序去重取前几
来源：http://ihy.jlsjyb.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ibv.gzhubu.top

[R52] 统计行数
来源：http://unv.bbcook.cn

wc -l a.txt
来源：http://zzz.316326.xyz

[R53] 查看文件头与实时尾
来源：http://uzw.gzhubu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iun.zhijiandao.cn

[R54] 比较两个文件
来源：http://xmy.svipenyu.cn

diff a.txt b.txt
来源：http://olf.cqqwz.cn

[R55] 压缩与解压
来源：http://usz.shanyushiyangtech.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zcl.dianchejie.cn

[R56] 远程拷贝
来源：http://xiy.svipenyu.cn

scp file user@host:/path/
来源：http://hsw.hnxiangtu.top

[R57] 远程执行命令
来源：http://iof.kuanghao11.cn

ssh user@host 'uptime'
来源：http://lra.kuanghao11.cn

[R58] 下载文件
来源：http://nin.zhiwuduotai.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mwt.xylfe.cn

[R59] 发 POST JSON
来源：http://lsa.chenjidiqi.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gqn.hnxiangtu.top

[R60] 只看 HTTP 状态码
来源：http://oer.yueranfly.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yeq.xuanzx.com

[R61] 磁盘占用
来源：http://rrt.xingfuxueyuan.xyz

df -h;  du -sh *
来源：http://zja.zhongyouzk.top

[R62] 找最占空间的文件
来源：http://ven.haohaochexian.top

du -ah . | sort -rh | head -10
来源：http://lyf.hammf.cn

[R63] 内存与进程
来源：http://uua.pengpengdd.cyou

free -h;  ps aux | grep nginx
来源：http://myj.zhixingplan.top

[R64] 结束进程
来源：http://rrm.yj202588.top

kill -9 $(pgrep -f app.py)
来源：http://oit.smart0.xyz

[R65] 查看端口占用
来源：http://dhm.9152youxi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gej.zhoulong.xyz

[R66] 定时任务
来源：http://ubq.nwbrower.top

crontab -e;  crontab -l
来源：http://ebm.aibaodan.cn

[R67] 生成随机十六进制串
来源：http://oyd.zhixingplan.top

openssl rand -hex 16
来源：http://yzf.snrcjt.cn

[R68] 计算文件校验值
来源：http://ody.nanxuanxn.top

sha256sum a.txt;  md5sum a.txt
来源：http://mfa.jinqigufen.top

[R69] 生成随机密码
来源：http://cno.svipenyu.cn

head -c 16 /dev/urandom | base64
来源：http://pwy.daria6918.cn

[R70] 时间戳与互转
来源：http://qem.gotoacloud.top

date +%s;  date -d @1700000000
来源：http://sgr.xziqi.cn

[R71] 日期格式化
来源：http://jap.c1oappe.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://tnb.daxiang520.top

[R72] 等待端口就绪
来源：http://glx.hysaishi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://piz.jlsjyb.cn

[R73] 分割大日志
来源：http://cec.xuetiantiany.cn

split -l 1000 big.log part_
来源：http://zwx.zdqjudy.top

[R74] 批量重命名
来源：http://bkz.hesvh.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ryt.xuanzx.com

[R75] 导出环境变量
来源：http://ecl.jinghuilouyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://xze.yanxiufei.cn

[R76] 使用临时文件
来源：http://zeh.birdmap.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dbh.jinyuanbaomall.cn

[R77] 读取用户输入
来源：http://dzj.pycfn.com

read -rp "请输入: " ans
来源：http://uue.xylfe.cn

[R78] 交互式菜单
来源：http://qiz.uphjek.com

select opt in a b c; do echo "$opt"; break; done
来源：http://oiy.shuidangran.top

[R79] 解析命令行选项
来源：http://dvc.tianlin.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://obd.ctjpmb.com

[R80] 查看脚本执行耗时
来源：http://vlw.pengpengdd.cyou

time ./run.sh
来源：http://ohq.tanke756.top

================================================================================
来源：http://pfj.zhengqikj.top

S. C / C++ 专题
来源：http://gmv.tarul.cn

================================================================================
来源：http://fjn.fehbvm.com

[S01] C：Hello World
来源：http://hig.jyoumei.cn

#include <stdio.h>
来源：http://clh.cqqwz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://lvi.iojbl.cn

[S02] C：变量与格式化输出
来源：http://gwr.chenjidiqi.icu

int a = 10; printf("%d\n", a);
来源：http://zlq.daxiang520.top

[S03] C：读入整数
来源：http://yfk.jyoumei.cn

int x; scanf("%d", &x);
来源：http://vsb.xylfe.cn

[S04] C：字符串复制
来源：http://zih.sweek.top

char dst[32]; strcpy(dst, "hi");
来源：http://wcj.yj20258.top

[S05] C：字符串长度
来源：http://aix.sufxvd.cn

strlen(s)
来源：http://jcp.svipenyu.cn

[S06] C：字符串比较
来源：http://gzg.9152youxi.cn

strcmp(a, b) == 0
来源：http://uzj.yuanzhike.top

[S07] C：数组遍历求和
来源：http://drk.cdnleiting.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mum.pycfn.com

[S08] C：动态内存分配与释放
来源：http://hnx.sufxvd.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hqh.dianchejie.cn

[S09] C：结构体定义与初始化
来源：http://ipy.pengpengdd.cyou

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vxp.pengpengdd.cyou

[S10] C：指针与解引用
来源：http://rvt.fktsv.cn

int *p = &a;  *p = 5;
来源：http://lom.jianghu66.top

[S11] C：逐行读文件
来源：http://yjs.jinqigufen.top

FILE *f = fopen("a.txt", "r");
来源：http://ved.tarul.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://fqo.hcnkem.com

fclose(f);
来源：http://cwq.xylfe.cn

[S12] C：写文件
来源：http://cko.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wlj.jqgfzy.top

[S13] C：宏定义
来源：http://vld.ivvv.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://six.ywan-chungtsiang.top

[S14] C：枚举
来源：http://pfl.vqdsnc.cn

enum Color { RED, GREEN, BLUE };
来源：http://gzg.cdnleiting.top

[S15] C：类型转换
来源：http://hhc.kuanghao11.cn

(double) a / b
来源：http://eup.kuanghao11.cn

[S16] C：位操作置位
来源：http://atl.ivvv.top

x |= (1 << 3);
来源：http://suo.jlsjyb.cn

[S17] C：安全拼接字符串
来源：http://xle.tian-w.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://umv.xziqi.cn

[S18] C：命令行参数
来源：http://ede.hfpthk.cn

int main(int argc, char **argv)
来源：http://cjk.gaohongyu789.top

[S19] C：快速排序
来源：http://grf.pengpengdd.cyou

qsort(a, n, sizeof(int), cmp);
来源：http://fbw.tarul.cn

[S20] C：二分查找
来源：http://fvg.hcnkem.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tnd.yonumen.top

[S21] C：字符类别判断
来源：http://dtx.gotoacloud.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jpn.nwbrower.top

[S22] C：字符串转数字
来源：http://iqt.tianlin.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://ocw.wangshuangyany.cn

[S23] C：随机数
来源：http://oyo.yj20258888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xma.dashuyun.cn

[S24] C：获取本地时间
来源：http://gvx.zycfv.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zmj.ywan-chungtsiang.top

[S25] C：内存拷贝
来源：http://add.quarkkingdee.top

memcpy(dst, src, n);
来源：http://ijn.hesvh.cn

[S26] C：内存清零
来源：http://qdc.ppjwa.cn

memset(a, 0, sizeof a);
来源：http://mfw.zhaomingkeji.xyz

[S27] C：定义常量
来源：http://cfe.wangdashe.top

const double PI = 3.14159;
来源：http://fly.iojbl.cn

[S28] C：静态变量
来源：http://aht.chenlongwang.top

static int counter = 0;
来源：http://cdj.zdqjudy.top

[S29] C：变参函数
来源：http://vil.jlsjyb.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fhg.zhoulong.xyz

[S30] C：头文件保护
来源：http://msi.snrcjt.cn

#ifndef X_H
来源：http://ziy.xylfe.cn

#define X_H
来源：http://gub.meibo888.top

#endif
来源：http://pcd.zhaomingkeji.xyz

[S31] C++：Hello World
来源：http://pre.cheryme.top

#include <iostream>
来源：http://kim.9152youxi.cn

int main() { std::cout << "Hello\n"; }
来源：http://wob.ppjwa.cn

[S32] C++：字符串
来源：http://wpm.wangdashe.top

std::string s = "hi";  s += "!";
来源：http://ljs.nwbrower.top

[S33] C++：vector 增删
来源：http://xzr.hongshengwenyu.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qnp.jlsjyb.cn

[S34] C++：遍历 vector
来源：http://fws.yueranfly.top

for (auto &x : v) { std::cout << x; }
来源：http://egt.ppjwa.cn

[S35] C++：map
来源：http://pvh.316326.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fma.zhixingplan.top

[S36] C++：unordered_map
来源：http://kco.iojbl.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rek.hysaishi.cn

[S37] C++：set
来源：http://qib.gogol.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tkj.epnwcf.com

[S38] C++：排序
来源：http://wnw.vqdsnc.cn

std::sort(v.begin(), v.end());
来源：http://gvq.hongshengwenyu.top

[S39] C++：自定义比较器排序
来源：http://cxd.316326.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cit.tian-w.cn

[S40] C++：查找元素
来源：http://xbq.yuanzhike.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jwa.gaohongyu789.top

[S41] C++：类与构造函数
来源：http://awc.yueranfly.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qnt.ybcxt.top

[S42] C++：继承与虚函数
来源：http://imm.daria6918.cn

class B : public Base { public: void f() override {} };
来源：http://pxu.cheryme.top

[S43] C++：智能指针
来源：http://hvd.zdqjudy.top

auto p = std::make_unique<int>(5);
来源：http://coz.feifeiyinyue.top

[S44] C++：引用传参
来源：http://sac.snrcjt.cn

void inc(int &x) { ++x; }
来源：http://qui.tarul.cn

[S45] C++：lambda
来源：http://naz.shanyushiyangtech.top

auto add = [](int a, int b) { return a + b; };
来源：http://yvw.pengpengdd.cyou

[S46] C++：函数模板
来源：http://neg.wangshuangyany.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kff.sweek.top

[S47] C++：结构化绑定遍历
来源：http://kqn.yuanzhike.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dbu.yongpay.top

[S48] C++：逐行读文件
来源：http://qfx.yanxiufei.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nee.hysaishi.cn

while (std::getline(in, line)) { }
来源：http://gcc.shanyushiyangtech.top

[S49] C++：写文件
来源：http://uxo.nanxuanxn.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mzw.vqdsnc.cn

[S50] C++：格式化数字
来源：http://psn.cucudq.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zdi.andypj.xyz

[S51] C++：显式类型转换
来源：http://qhb.cdnleiting.top

static_cast<double>(a) / b
来源：http://tei.zycfv.cn

[S52] C++：const 与 noexcept
来源：http://emf.fanxiaobao.xyz

int size() const noexcept { return n_; }
来源：http://ehz.jiagoushi.top

[S53] C++：移动语义
来源：http://lqd.fktsv.cn

std::vector<int> w = std::move(v);
来源：http://ykf.xuetiantiany.cn

[S54] C++：异常处理
来源：http://eyu.dianchejie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xeq.jiagoushi.top

[S55] C++：结构化绑定
来源：http://esu.cucudq.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xzp.xziqi.cn

[S56] C++：optional
来源：http://lps.aizwys.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://jrf.gaohongyu789.top

[S57] C++：编译期常量
来源：http://xmj.bbcook.cn

constexpr int N = 10;
来源：http://ltv.sxryk.cn

[S58] C++：命名空间
来源：http://hoo.0kj1m.cn

namespace ns { int f() { return 1; } }
来源：http://sgv.jqgufenzy.top

[S59] C++：静态断言
来源：http://vfw.shuidangran.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://rtx.wangdashe.top

[S60] C++：遍历并删除元素
来源：http://vrl.yuanzhike.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ezi.9152youxi.cn

================================================================================
来源：http://yaf.hywenlv.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fak.xuanzx.com

================================================================================
来源：http://ecn.guowangkeji.top

[T01] Kotlin：Hello World
来源：http://zwc.daxiang520.top

println("Hello")
来源：http://vpc.epnwcf.com

[T02] Kotlin：变量
来源：http://xci.hfpthk.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iem.sufxvd.cn

[T03] Kotlin：字符串模板
来源：http://bla.aizwys.cn

"值: $b"
来源：http://jav.sysykeji.top

[T04] Kotlin：空安全
来源：http://xah.pycfn.com

val n: String? = null;  n?.length
来源：http://ldo.zhengqikj.top

[T05] Kotlin：when 表达式
来源：http://dah.xuetiantiany.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bqn.zhixingplan.top

[T06] Kotlin：集合映射
来源：http://fqg.xingfuxueyuan.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://xxi.yj20258888.top

[T07] Kotlin：集合过滤
来源：http://upx.jinqigufen.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://sej.andypj.xyz

[T08] Kotlin：数据类
来源：http://qij.chenlongwang.top

data class User(val name: String, val age: Int)
来源：http://muq.zhengqikj.top

[T09] Kotlin：扩展函数
来源：http://jmd.fehbvm.com

fun String.exclaim() = this + "!"
来源：http://eqn.gzhubu.top

[T10] Kotlin：默认参数
来源：http://cwa.316326.xyz

fun greet(name: String = "World") = "Hi $name"
来源：http://ghp.hesvh.cn


<!-- 参考信息 -->