代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mug.cqqwz.cn

[R10] 正则匹配
来源：http://kdw.yanxiufei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kvf.ydzc1.top

[R11] case 多分支
来源：http://hyj.sxryk.cn

case "$1" in
来源：http://tcy.yanxiufei.cn

start) echo "启动" ;;
来源：http://fgk.wangdashe.top

stop)  echo "停止" ;;
来源：http://ziw.ywan-chungtsiang.top

*)     echo "未知命令" ;;
来源：http://oth.ehwqpu.com

esac
来源：http://xzt.zycfv.cn

[R12] for 遍历文件
来源：http://fup.cdnleiting.top

for f in *.txt; do echo "$f"; done
来源：http://mgg.cqqwz.cn

[R13] for 计数循环
来源：http://bqc.yongpay.top

for i in {1..10}; do echo "$i"; done
来源：http://yot.jianghu66.top

[R14] C 风格 for
来源：http://tbf.shzxlz.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xox.havefunace.top

[R15] while 逐行读文件
来源：http://bku.daria6918.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ate.aizwys.cn

[R16] until 等待条件
来源：http://gdt.zhoulong.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wze.fengsongda.top

[R17] 数组定义与取值
来源：http://izm.ivvv.top

arr=(a b c); echo "${arr[0]}"
来源：http://nod.9152youxi.cn

[R18] 遍历数组
来源：http://bxa.tian-w.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cqf.xingfuxueyuan.xyz

[R19] 数组长度
来源：http://sbm.yanxiufei.cn

echo "${#arr[@]}"
来源：http://ffk.sysykeji.top

[R20] 关联数组（字典）
来源：http://wuq.jyoumei.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lpg.fanxiaobao.xyz

[R21] 字符串长度
来源：http://kul.yj202588.top

echo "${#s}"
来源：http://can.epnwcf.com

[R22] 截取子串
来源：http://hca.bbcook.cn

echo "${s:0:5}"
来源：http://zrs.gzhubu.top

[R23] 字符串替换
来源：http://cff.pengpengdd.cyou

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://uod.xingfuxueyuan.xyz

[R24] 大小写转换
来源：http://esf.wangshuangyany.cn

echo "${s^^}"; echo "${s,,}"
来源：http://aht.ehwqpu.com

[R25] 去后缀 / 去前缀
来源：http://uef.uphjek.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://qpz.zdqjudy.top

[R26] 命令替换
来源：http://wen.gzhubu.top

now=$(date +%F); echo "$now"
来源：http://elt.meibo888.top

[R27] 算术展开
来源：http://zgj.guannengcc.top

echo $((1 + 2 * 3))
来源：http://xfc.yuanzhike.top

[R28] 浮点运算
来源：http://let.svipenyu.cn

echo "scale=2; 10/3" | bc
来源：http://kxz.shuidangran.top

[R29] 定义函数
来源：http://bga.gotoacloud.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ypg.yuanzhike.top

[R30] 函数返回状态码
来源：http://cpm.vehdjk.com

f() { return 0; }; f || echo "失败了"
来源：http://abq.ehwqpu.com

[R31] 局部变量
来源：http://wwe.tanke756.top

f() { local x=1; echo "$x"; }
来源：http://maj.yfazqb.com

[R32] 参数个数校验
来源：http://cjm.aibaodan.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://jfv.guannengcc.top

[R33] 捕获错误并提示行号
来源：http://dhz.jlsjyb.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cft.nwbrower.top

[R34] 退出时清理
来源：http://gqo.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://wvh.yuxming.cn

[R35] 后台执行并等待
来源：http://wzr.yuxming.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://hry.smart0.xyz

[R36] 并发执行多个任务
来源：http://gyl.hongshengwenyu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lav.andypj.xyz

[R37] 把输出赋给变量
来源：http://ulh.feifeiyinyue.top

files=$(ls -1)
来源：http://utm.fanxiaobao.xyz

[R38] 管道串联
来源：http://dxb.ppjwa.cn

cat a.txt | grep -i error | wc -l
来源：http://unv.tian-w.cn

[R39] 重定向标准输出与错误
来源：http://jzi.haohaochexian.top

cmd > out.log 2>&1
来源：http://mqc.sufxvd.cn

[R40] 追加写日志
来源：http://stq.quarkkingdee.top

echo "log" >> out.log
来源：http://tlw.jqgufenzy.top

[R41] 丢弃输出
来源：http://elz.cucudq.cn

cmd >/dev/null 2>&1
来源：http://grq.xinyue.icu

[R42] 输入重定向
来源：http://pzd.jianghu66.top

wc -l < a.txt
来源：http://lcq.shzxlz.cn

[R43] 按名字查找文件
来源：http://cvl.snrcjt.cn

find . -name "*.log" -type f
来源：http://lev.yfazqb.com

[R44] 按修改时间查找
来源：http://tbs.zhixingplan.top

find . -mtime -7 -type f
来源：http://rlf.chenzaomai.com

[R45] 批量删除
来源：http://vfm.cdnleiting.top

find . -name "*.tmp" -delete
来源：http://upg.ybcxt.top

[R46] 递归替换文件内容
来源：http://bkh.guowangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bed.sweek.top

[R47] sed 单行替换
来源：http://wim.zhoulong.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://jsf.hnqzz.top

[R48] awk 取指定列
来源：http://orc.xinyue.icu

awk '{print $1, $3}' a.txt
来源：http://xyp.shanyushiyangtech.top

[R49] awk 带条件
来源：http://ius.fengsongda.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mxq.tian-w.cn

[R50] awk 求和
来源：http://pqq.zhoulong.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://swc.xziqi.cn

[R51] 排序去重取前几
来源：http://bdv.yj20258888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pid.fehbvm.com

[R52] 统计行数
来源：http://hfk.0kj1m.cn

wc -l a.txt
来源：http://dil.feifeiyinyue.top

[R53] 查看文件头与实时尾
来源：http://hwb.yanxiufei.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lqy.shangyingyoupin.top

[R54] 比较两个文件
来源：http://ghq.tian-w.cn

diff a.txt b.txt
来源：http://nkx.yonumen.top

[R55] 压缩与解压
来源：http://awp.vehdjk.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://grg.epnwcf.com

[R56] 远程拷贝
来源：http://yym.ydjk.org.cn

scp file user@host:/path/
来源：http://pfv.zdbjq.cn

[R57] 远程执行命令
来源：http://nut.0kj1m.cn

ssh user@host 'uptime'
来源：http://noc.ybcxt.top

[R58] 下载文件
来源：http://qkx.ydjk.org.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eei.zhongyouzk.top

[R59] 发 POST JSON
来源：http://xdw.uphjek.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zxf.hnxiangtu.top

[R60] 只看 HTTP 状态码
来源：http://qul.cheryme.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nvg.birdmap.top

[R61] 磁盘占用
来源：http://hvl.fanxiaobao.xyz

df -h;  du -sh *
来源：http://usd.shuidangran.top

[R62] 找最占空间的文件
来源：http://toa.wangshuangyany.cn

du -ah . | sort -rh | head -10
来源：http://mhs.yvedp.cn

[R63] 内存与进程
来源：http://ifi.ydjk.org.cn

free -h;  ps aux | grep nginx
来源：http://cfh.9152youxi.cn

[R64] 结束进程
来源：http://jng.feifeiyinyue.top

kill -9 $(pgrep -f app.py)
来源：http://vwc.fengsongda.top

[R65] 查看端口占用
来源：http://kfj.sufxvd.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wue.sysykeji.top

[R66] 定时任务
来源：http://bog.fengsongda.top

crontab -e;  crontab -l
来源：http://nns.tianlin.xyz

[R67] 生成随机十六进制串
来源：http://tin.hfpthk.cn

openssl rand -hex 16
来源：http://cdj.daxiang520.top

[R68] 计算文件校验值
来源：http://ztu.yanxiufei.cn

sha256sum a.txt;  md5sum a.txt
来源：http://cgd.yj20258888.top

[R69] 生成随机密码
来源：http://tmg.jinqigufen.top

head -c 16 /dev/urandom | base64
来源：http://geg.hesvh.cn

[R70] 时间戳与互转
来源：http://thq.zhaomingkeji.xyz

date +%s;  date -d @1700000000
来源：http://slg.fehbvm.com

[R71] 日期格式化
来源：http://jfi.jiagoushi.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://sxe.aizwys.cn

[R72] 等待端口就绪
来源：http://xhl.jqgfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://cmw.pengpengdd.cyou

[R73] 分割大日志
来源：http://xin.zhoulong.xyz

split -l 1000 big.log part_
来源：http://hra.andypj.xyz

[R74] 批量重命名
来源：http://rcz.zhongyouzk.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://zgq.gaohongyu789.top

[R75] 导出环境变量
来源：http://hri.wangdashe.top

export PATH="$HOME/bin:$PATH"
来源：http://emi.ydjk.org.cn

[R76] 使用临时文件
来源：http://mcn.svipenyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wkd.yonumen.top

[R77] 读取用户输入
来源：http://hcw.wangshuangyany.cn

read -rp "请输入: " ans
来源：http://qtp.svipenyu.cn

[R78] 交互式菜单
来源：http://vkr.havefunace.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xzh.daxiang520.top

[R79] 解析命令行选项
来源：http://mvl.cdnleiting.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zcs.bbcook.cn

[R80] 查看脚本执行耗时
来源：http://zme.zhaomingkeji.xyz

time ./run.sh
来源：http://bdp.xylfe.cn

================================================================================
来源：http://uue.hfpthk.cn

S. C / C++ 专题
来源：http://vvc.cheryme.top

================================================================================
来源：http://ovp.sysykeji.top

[S01] C：Hello World
来源：http://vhq.nwbrower.top

#include <stdio.h>
来源：http://xvp.yongpay.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fcs.dianchejie.cn

[S02] C：变量与格式化输出
来源：http://kkt.epnwcf.com

int a = 10; printf("%d\n", a);
来源：http://jwc.tarul.cn

[S03] C：读入整数
来源：http://yyv.nanxinkj.top

int x; scanf("%d", &x);
来源：http://gwn.ppjwa.cn

[S04] C：字符串复制
来源：http://vmi.yj202588.top

char dst[32]; strcpy(dst, "hi");
来源：http://lju.jqgfzy.top

[S05] C：字符串长度
来源：http://bms.ppjwa.cn

strlen(s)
来源：http://vwh.daxiang520.top

[S06] C：字符串比较
来源：http://qeo.guannengcc.top

strcmp(a, b) == 0
来源：http://lck.sjlbkw.cn

[S07] C：数组遍历求和
来源：http://bzt.snrcjt.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pfc.tanke756.top

[S08] C：动态内存分配与释放
来源：http://vcj.cucudq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gtp.quarkkingdee.top

[S09] C：结构体定义与初始化
来源：http://rgs.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pjj.shanyushiyangtech.top

[S10] C：指针与解引用
来源：http://efa.zhoulong.xyz

int *p = &a;  *p = 5;
来源：http://qpy.ydzc1.top

[S11] C：逐行读文件
来源：http://skj.jinqigfzy.top

FILE *f = fopen("a.txt", "r");
来源：http://teh.fengsongda.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mje.zdqjudy.top

fclose(f);
来源：http://vng.hnxiangtu.top

[S12] C：写文件
来源：http://ybu.yangfankeji.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jzp.jinghuilouyu.cn

[S13] C：宏定义
来源：http://jhb.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qyv.wangshuangyany.cn

[S14] C：枚举
来源：http://yed.zhengqikj.top

enum Color { RED, GREEN, BLUE };
来源：http://mnh.meibo888.top

[S15] C：类型转换
来源：http://qpt.yanxiufei.cn

(double) a / b
来源：http://fka.jlsjyb.cn

[S16] C：位操作置位
来源：http://isq.yangfankeji.com

x |= (1 << 3);
来源：http://scp.bbcook.cn

[S17] C：安全拼接字符串
来源：http://xkq.shzxlz.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jts.hysaishi.cn

[S18] C：命令行参数
来源：http://xfm.9152youxi.cn

int main(int argc, char **argv)
来源：http://smf.ybcxt.top

[S19] C：快速排序
来源：http://cvp.52xcode.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nqs.redwolf501.top

[S20] C：二分查找
来源：http://xez.fehbvm.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bxg.gogol.net.cn

[S21] C：字符类别判断
来源：http://fgq.zhoulong.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gpj.yongpay.top

[S22] C：字符串转数字
来源：http://uan.jiagoushi.top

atoi("42");  strtod("3.14", NULL);
来源：http://aco.hcnkem.com

[S23] C：随机数
来源：http://ggy.yj20258888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://nwk.zdqjudy.top

[S24] C：获取本地时间
来源：http://yxa.chenlongwang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xay.hesvh.cn

[S25] C：内存拷贝
来源：http://izd.chenjidiqi.icu

memcpy(dst, src, n);
来源：http://dqe.jiagoushi.top

[S26] C：内存清零
来源：http://ptq.chenzaomai.com

memset(a, 0, sizeof a);
来源：http://mwm.zhijiandao.cn

[S27] C：定义常量
来源：http://cxg.shzxlz.cn

const double PI = 3.14159;
来源：http://egz.nanxinkj.top

[S28] C：静态变量
来源：http://uub.gzhubu.top

static int counter = 0;
来源：http://vfx.jinghuilouyu.cn

[S29] C：变参函数
来源：http://opo.bbcook.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sdc.ppjwa.cn

[S30] C：头文件保护
来源：http://wdi.zhoulong.xyz

#ifndef X_H
来源：http://gdf.jinyuanbaomall.cn

#define X_H
来源：http://ryo.0kj1m.cn

#endif
来源：http://fvp.xziqi.cn

[S31] C++：Hello World
来源：http://zxq.shanyushiyangkeji.top

#include <iostream>
来源：http://mjm.cqqwz.cn

int main() { std::cout << "Hello\n"; }
来源：http://agt.c1oappe.top

[S32] C++：字符串
来源：http://qeq.chenzaomai.com

std::string s = "hi";  s += "!";
来源：http://ghv.xinyue.icu

[S33] C++：vector 增删
来源：http://fyw.fengsongda.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fnh.dashuyun.cn

[S34] C++：遍历 vector
来源：http://lti.shzxlz.cn

for (auto &x : v) { std::cout << x; }
来源：http://zyq.andypj.xyz

[S35] C++：map
来源：http://jyh.hfpthk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://thb.xziqi.cn

[S36] C++：unordered_map
来源：http://lik.cheryme.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xgd.ydjk.org.cn

[S37] C++：set
来源：http://nkp.cqqwz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vzj.hnqzz.top

[S38] C++：排序
来源：http://don.yonumen.top

std::sort(v.begin(), v.end());
来源：http://wbf.c1oappe.top

[S39] C++：自定义比较器排序
来源：http://qjl.316326.xyz

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tjj.jqgufenzy.top

[S40] C++：查找元素
来源：http://pdi.zdbjq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rno.fehbvm.com

[S41] C++：类与构造函数
来源：http://ful.fktsv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://usm.fktsv.cn

[S42] C++：继承与虚函数
来源：http://bgp.chenlongwang.top

class B : public Base { public: void f() override {} };
来源：http://fjf.zdbjq.cn

[S43] C++：智能指针
来源：http://scg.daxiang520.top

auto p = std::make_unique<int>(5);
来源：http://vrv.hysaishi.cn

[S44] C++：引用传参
来源：http://klz.daria6918.cn

void inc(int &x) { ++x; }
来源：http://wzm.zhiwuduotai.top

[S45] C++：lambda
来源：http://xfb.fktsv.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bod.zhaomingkeji.xyz

[S46] C++：函数模板
来源：http://hej.sjlbkw.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tea.xingfuxueyuan.xyz

[S47] C++：结构化绑定遍历
来源：http://vts.birdmap.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pch.shanyushiyangkeji.top

[S48] C++：逐行读文件
来源：http://ysk.sjlbkw.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vks.gogol.net.cn

while (std::getline(in, line)) { }
来源：http://zmq.9152youxi.cn

[S49] C++：写文件
来源：http://llf.pycfn.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xwq.fktsv.cn

[S50] C++：格式化数字
来源：http://qlf.zhijiandao.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cyj.jinghuilouyu.cn

[S51] C++：显式类型转换
来源：http://xue.gogol.net.cn

static_cast<double>(a) / b
来源：http://abk.yvedp.cn

[S52] C++：const 与 noexcept
来源：http://zpp.52xcode.cn

int size() const noexcept { return n_; }
来源：http://ygf.nwbrower.top

[S53] C++：移动语义
来源：http://imw.yueranfly.top

std::vector<int> w = std::move(v);
来源：http://swg.9152youxi.cn

[S54] C++：异常处理
来源：http://aoa.fanxiaobao.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ynw.snrcjt.cn

[S55] C++：结构化绑定
来源：http://dlf.chenjidiqi.icu

auto [a, b] = std::make_pair(1, 2);
来源：http://vcs.gaohongyu789.top

[S56] C++：optional
来源：http://shp.hongshengwenyu.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vyr.sysykeji.top

[S57] C++：编译期常量
来源：http://qbd.gogol.net.cn

constexpr int N = 10;
来源：http://rwe.shanyushiyangtech.top

[S58] C++：命名空间
来源：http://yjw.ppjwa.cn

namespace ns { int f() { return 1; } }
来源：http://qpb.havefunace.top

[S59] C++：静态断言
来源：http://qfx.sweek.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qem.nanxuanxn.top

[S60] C++：遍历并删除元素
来源：http://jsm.feifeiyinyue.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nvv.sjlbkw.cn

================================================================================
来源：http://okn.ywan-chungtsiang.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pho.wangdashe.top

================================================================================
来源：http://mds.chenzaomai.com

[T01] Kotlin：Hello World
来源：http://ifo.52xcode.cn

println("Hello")
来源：http://bqq.guowangkeji.top

[T02] Kotlin：变量
来源：http://cbp.smart0.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wcb.zhaomingkeji.xyz

[T03] Kotlin：字符串模板
来源：http://wev.tian-w.cn

"值: $b"
来源：http://rue.sufxvd.cn

[T04] Kotlin：空安全
来源：http://pkc.vehdjk.com

val n: String? = null;  n?.length
来源：http://hgu.shuidangran.top

[T05] Kotlin：when 表达式
来源：http://jtt.zdbjq.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hzw.guowangkeji.top

[T06] Kotlin：集合映射
来源：http://uzj.zhijiandao.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fdo.sjlbkw.cn

[T07] Kotlin：集合过滤
来源：http://yox.ybcxt.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mqc.feifeiyinyue.top

[T08] Kotlin：数据类
来源：http://plu.xziqi.cn

data class User(val name: String, val age: Int)
来源：http://cru.jlsjyb.cn

[T09] Kotlin：扩展函数
来源：http://ksh.shangyingyoupin.top

fun String.exclaim() = this + "!"
来源：http://elk.sjlbkw.cn

[T10] Kotlin：默认参数
来源：http://kjz.zhixingplan.top

fun greet(name: String = "World") = "Hi $name"
来源：http://iag.jinghuilouyu.cn


<!-- 参考信息 -->