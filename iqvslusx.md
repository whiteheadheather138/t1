代发 wailian999

readonly PI=3.14
来源：http://bwm.c1oappe.top

[R04] 位置参数
来源：http://dro.yanxiufei.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pxu.yvedp.cn

[R05] 参数默认值
来源：http://xbl.yj20258.top

name="${1:-default}"
来源：http://evp.jyoumei.cn

[R06] 判断命令是否存在
来源：http://oea.cheryme.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mlg.ybcxt.top

[R07] if 判断文件
来源：http://jcd.zhongyouzk.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mzu.tarul.cn

[R08] 数值比较
来源：http://ipi.xinyue.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://eld.snrcjt.cn

[R09] 字符串比较
来源：http://xox.bbcook.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hrr.jlsjyb.cn

[R10] 正则匹配
来源：http://tvh.gotoacloud.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://kgz.yj202588.top

[R11] case 多分支
来源：http://ymn.sufxvd.cn

case "$1" in
来源：http://fsx.jqgfzy.top

start) echo "启动" ;;
来源：http://miq.gaohongyu789.top

stop)  echo "停止" ;;
来源：http://vwe.bjfxy.top

*)     echo "未知命令" ;;
来源：http://zwq.jinghuilouyu.cn

esac
来源：http://xei.hongshengwenyu.top

[R12] for 遍历文件
来源：http://rds.sjlbkw.cn

for f in *.txt; do echo "$f"; done
来源：http://bod.svipenyu.cn

[R13] for 计数循环
来源：http://nlq.hnxiangtu.top

for i in {1..10}; do echo "$i"; done
来源：http://ojs.zhijiandao.cn

[R14] C 风格 for
来源：http://wbn.zdqjudy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ipw.chenjidiqi.icu

[R15] while 逐行读文件
来源：http://uti.shanyushiyangkeji.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fko.xylfe.cn

[R16] until 等待条件
来源：http://nfl.daria6918.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lmm.andypj.xyz

[R17] 数组定义与取值
来源：http://epc.ydzc1.top

arr=(a b c); echo "${arr[0]}"
来源：http://omc.uphjek.com

[R18] 遍历数组
来源：http://pep.316326.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ujm.yueranfly.top

[R19] 数组长度
来源：http://oru.dashuyun.cn

echo "${#arr[@]}"
来源：http://bem.zhoulong.xyz

[R20] 关联数组（字典）
来源：http://tao.fanxiaobao.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://nkg.smart0.xyz

[R21] 字符串长度
来源：http://nap.hywenlv.cn

echo "${#s}"
来源：http://tls.hnxiangtu.top

[R22] 截取子串
来源：http://flr.epnwcf.com

echo "${s:0:5}"
来源：http://pwd.xylfe.cn

[R23] 字符串替换
来源：http://rpy.52xcode.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jij.cheryme.top

[R24] 大小写转换
来源：http://ltq.sufxvd.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hkv.zhongyouzk.top

[R25] 去后缀 / 去前缀
来源：http://mmg.smart0.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://phu.cucudq.cn

[R26] 命令替换
来源：http://ixp.vqdsnc.cn

now=$(date +%F); echo "$now"
来源：http://oft.nanxinkj.top

[R27] 算术展开
来源：http://xwo.yvedp.cn

echo $((1 + 2 * 3))
来源：http://xhs.yonumen.top

[R28] 浮点运算
来源：http://bef.pengpengdd.cyou

echo "scale=2; 10/3" | bc
来源：http://cmf.zdqjudy.top

[R29] 定义函数
来源：http://chy.yfazqb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://odl.zhixingplan.top

[R30] 函数返回状态码
来源：http://dlb.xinyue.icu

f() { return 0; }; f || echo "失败了"
来源：http://wgh.316326.xyz

[R31] 局部变量
来源：http://ggy.shanyushiyangkeji.top

f() { local x=1; echo "$x"; }
来源：http://ztt.havefunace.top

[R32] 参数个数校验
来源：http://sxs.xingfuxueyuan.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://udp.tianlin.xyz

[R33] 捕获错误并提示行号
来源：http://cwc.ivvv.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nnj.feifeiyinyue.top

[R34] 退出时清理
来源：http://tkr.cdnleiting.top

trap 'rm -f "$tmp"' EXIT
来源：http://nsr.sjlbkw.cn

[R35] 后台执行并等待
来源：http://ldh.ywan-chungtsiang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://moo.wangdashe.top

[R36] 并发执行多个任务
来源：http://gzh.gaohongyu789.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://bkq.hcnkem.com

[R37] 把输出赋给变量
来源：http://jfy.xinyue.icu

files=$(ls -1)
来源：http://buv.fengsongda.top

[R38] 管道串联
来源：http://qkz.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://cfp.ehwqpu.com

[R39] 重定向标准输出与错误
来源：http://teh.yj20258888.top

cmd > out.log 2>&1
来源：http://xsj.zhiwuduotai.top

[R40] 追加写日志
来源：http://ffp.xuanzx.com

echo "log" >> out.log
来源：http://knz.yvedp.cn

[R41] 丢弃输出
来源：http://bod.ybcxt.top

cmd >/dev/null 2>&1
来源：http://udm.mhx1999.top

[R42] 输入重定向
来源：http://oro.zhijiandao.cn

wc -l < a.txt
来源：http://abk.andypj.xyz

[R43] 按名字查找文件
来源：http://fwo.shzxlz.cn

find . -name "*.log" -type f
来源：http://hla.cashguo.top

[R44] 按修改时间查找
来源：http://ppk.zhaomingkeji.xyz

find . -mtime -7 -type f
来源：http://soq.jqgfzy.top

[R45] 批量删除
来源：http://bjq.zdqjudy.top

find . -name "*.tmp" -delete
来源：http://cvw.haohaochexian.top

[R46] 递归替换文件内容
来源：http://wjg.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wlw.chenlongwang.top

[R47] sed 单行替换
来源：http://niz.vqdsnc.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tee.ydzc1.top

[R48] awk 取指定列
来源：http://btn.vqdsnc.cn

awk '{print $1, $3}' a.txt
来源：http://ubj.zycfv.cn

[R49] awk 带条件
来源：http://vrb.jqgfzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tzu.ydjk.org.cn

[R50] awk 求和
来源：http://bnk.shuidangran.top

awk '{s += $2} END {print s}' a.txt
来源：http://tyq.guowangkeji.top

[R51] 排序去重取前几
来源：http://vco.tarul.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gdl.zhiwuduotai.top

[R52] 统计行数
来源：http://gvk.shanyushiyangtech.top

wc -l a.txt
来源：http://lzs.xingfuxueyuan.xyz

[R53] 查看文件头与实时尾
来源：http://xnn.bbcook.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://djg.iojbl.cn

[R54] 比较两个文件
来源：http://thc.jinqigufen.top

diff a.txt b.txt
来源：http://shk.bjfxy.top

[R55] 压缩与解压
来源：http://hfh.yvedp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uvo.sxryk.cn

[R56] 远程拷贝
来源：http://jbs.hesvh.cn

scp file user@host:/path/
来源：http://awh.jinghuilouyu.cn

[R57] 远程执行命令
来源：http://bys.sysykeji.top

ssh user@host 'uptime'
来源：http://vmm.yuanzhike.top

[R58] 下载文件
来源：http://bcd.xziqi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pvq.ybcxt.top

[R59] 发 POST JSON
来源：http://tbk.tianlin.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vok.aizwys.cn

[R60] 只看 HTTP 状态码
来源：http://cfp.jinghuilouyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://azh.yonumen.top

[R61] 磁盘占用
来源：http://hvb.jinqigfzy.top

df -h;  du -sh *
来源：http://bxu.hywenlv.cn

[R62] 找最占空间的文件
来源：http://cjr.xuetiantiany.cn

du -ah . | sort -rh | head -10
来源：http://qoy.yangfankeji.com

[R63] 内存与进程
来源：http://ggd.hongshengwenyu.top

free -h;  ps aux | grep nginx
来源：http://uoy.tarul.cn

[R64] 结束进程
来源：http://rsn.0kj1m.cn

kill -9 $(pgrep -f app.py)
来源：http://kpd.hesvh.cn

[R65] 查看端口占用
来源：http://kfx.aibaodan.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ngf.wangshuangyany.cn

[R66] 定时任务
来源：http://lef.316326.xyz

crontab -e;  crontab -l
来源：http://pak.daria6918.cn

[R67] 生成随机十六进制串
来源：http://eqx.dianchejie.cn

openssl rand -hex 16
来源：http://krk.xuetiantiany.cn

[R68] 计算文件校验值
来源：http://umg.fehbvm.com

sha256sum a.txt;  md5sum a.txt
来源：http://yxu.xinyue.icu

[R69] 生成随机密码
来源：http://iky.ywan-chungtsiang.top

head -c 16 /dev/urandom | base64
来源：http://shl.aibaodan.cn

[R70] 时间戳与互转
来源：http://prs.fehbvm.com

date +%s;  date -d @1700000000
来源：http://msw.zhaomingkeji.xyz

[R71] 日期格式化
来源：http://geo.svipenyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qaf.uphjek.com

[R72] 等待端口就绪
来源：http://txk.meibo888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jbn.yj20258.top

[R73] 分割大日志
来源：http://ekj.sjlbkw.cn

split -l 1000 big.log part_
来源：http://zjn.iojbl.cn

[R74] 批量重命名
来源：http://wtd.shzxlz.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://frj.hammf.cn

[R75] 导出环境变量
来源：http://tls.redwolf501.top

export PATH="$HOME/bin:$PATH"
来源：http://rrr.52xcode.cn

[R76] 使用临时文件
来源：http://qin.jyoumei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wzg.daxiang520.top

[R77] 读取用户输入
来源：http://qfy.yangfankeji.com

read -rp "请输入: " ans
来源：http://vut.zhiwuduotai.top

[R78] 交互式菜单
来源：http://aak.ctjpmb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://pve.ybcxt.top

[R79] 解析命令行选项
来源：http://jbt.snrcjt.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://idv.cqqwz.cn

[R80] 查看脚本执行耗时
来源：http://pbl.tarul.cn

time ./run.sh
来源：http://orc.shzxlz.cn

================================================================================
来源：http://hjb.c1oappe.top

S. C / C++ 专题
来源：http://wyg.ctjpmb.com

================================================================================
来源：http://njg.sjlbkw.cn

[S01] C：Hello World
来源：http://mop.chenlongwang.top

#include <stdio.h>
来源：http://mkb.0kj1m.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qla.shanyushiyangkeji.top

[S02] C：变量与格式化输出
来源：http://apf.ydzc1.top

int a = 10; printf("%d\n", a);
来源：http://fhf.aibaodan.cn

[S03] C：读入整数
来源：http://xkg.daxiang520.top

int x; scanf("%d", &x);
来源：http://kqf.hysaishi.cn

[S04] C：字符串复制
来源：http://yuz.quarkkingdee.top

char dst[32]; strcpy(dst, "hi");
来源：http://wxv.zhaomingkeji.xyz

[S05] C：字符串长度
来源：http://lom.hongshengwenyu.top

strlen(s)
来源：http://ygk.haohaochexian.top

[S06] C：字符串比较
来源：http://hjc.guowangkeji.top

strcmp(a, b) == 0
来源：http://aih.sysykeji.top

[S07] C：数组遍历求和
来源：http://stv.yueranfly.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nos.ybcxt.top

[S08] C：动态内存分配与释放
来源：http://jua.yueranfly.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cae.gaohongyu789.top

[S09] C：结构体定义与初始化
来源：http://sui.pengpengdd.cyou

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://eus.jqgufenzy.top

[S10] C：指针与解引用
来源：http://cyb.yonumen.top

int *p = &a;  *p = 5;
来源：http://nlj.yvedp.cn

[S11] C：逐行读文件
来源：http://jij.yanxiufei.cn

FILE *f = fopen("a.txt", "r");
来源：http://can.havefunace.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://fzx.nanxuanxn.top

fclose(f);
来源：http://unf.gzhubu.top

[S12] C：写文件
来源：http://sik.yueranfly.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vzm.jqgfzy.top

[S13] C：宏定义
来源：http://ntt.tanke756.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eay.ydzc1.top

[S14] C：枚举
来源：http://qic.yuxming.cn

enum Color { RED, GREEN, BLUE };
来源：http://yie.cheryme.top

[S15] C：类型转换
来源：http://bwe.vqdsnc.cn

(double) a / b
来源：http://lpj.bjfxy.top

[S16] C：位操作置位
来源：http://lac.hnqzz.top

x |= (1 << 3);
来源：http://xtc.daria6918.cn

[S17] C：安全拼接字符串
来源：http://vdm.xylfe.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rfe.gzhubu.top

[S18] C：命令行参数
来源：http://wqr.yonumen.top

int main(int argc, char **argv)
来源：http://bkr.chenzaomai.com

[S19] C：快速排序
来源：http://gqu.ehwqpu.com

qsort(a, n, sizeof(int), cmp);
来源：http://zfy.sysykeji.top

[S20] C：二分查找
来源：http://bqw.ehwqpu.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bpp.zhengqikj.top

[S21] C：字符类别判断
来源：http://lwy.316326.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cdj.xuetiantiany.cn

[S22] C：字符串转数字
来源：http://yhn.dashuyun.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ysr.fehbvm.com

[S23] C：随机数
来源：http://nke.ybcxt.top

srand(time(NULL));  int r = rand() % 100;
来源：http://hey.feifeiyinyue.top

[S24] C：获取本地时间
来源：http://gqh.nanxinkj.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wjm.zhengqikj.top

[S25] C：内存拷贝
来源：http://ext.zycfv.cn

memcpy(dst, src, n);
来源：http://dqb.chenzaomai.com

[S26] C：内存清零
来源：http://bwi.redwolf501.top

memset(a, 0, sizeof a);
来源：http://wwp.yvedp.cn

[S27] C：定义常量
来源：http://izc.sweek.top

const double PI = 3.14159;
来源：http://lys.cheryme.top

[S28] C：静态变量
来源：http://lnv.gzhubu.top

static int counter = 0;
来源：http://zeg.yj20258.top

[S29] C：变参函数
来源：http://gme.hongshengwenyu.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://pyr.zhaomingkeji.xyz

[S30] C：头文件保护
来源：http://axi.tanke756.top

#ifndef X_H
来源：http://dny.jianghu66.top

#define X_H
来源：http://foo.hfpthk.cn

#endif
来源：http://tyx.jiagoushi.top

[S31] C++：Hello World
来源：http://zve.fengsongda.top

#include <iostream>
来源：http://nkw.yvedp.cn

int main() { std::cout << "Hello\n"; }
来源：http://wch.yfazqb.com

[S32] C++：字符串
来源：http://mtd.shanyushiyangkeji.top

std::string s = "hi";  s += "!";
来源：http://usj.cqqwz.cn

[S33] C++：vector 增删
来源：http://ngw.jinghuilouyu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gwa.pycfn.com

[S34] C++：遍历 vector
来源：http://hsp.yvedp.cn

for (auto &x : v) { std::cout << x; }
来源：http://eje.fzhhl.top

[S35] C++：map
来源：http://ycz.cdnleiting.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zak.jlsjyb.cn

[S36] C++：unordered_map
来源：http://pqj.tanke756.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xag.chenzaomai.com

[S37] C++：set
来源：http://dqg.shuidangran.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cml.sweek.top

[S38] C++：排序
来源：http://kjw.fengsongda.top

std::sort(v.begin(), v.end());
来源：http://ota.hammf.cn

[S39] C++：自定义比较器排序
来源：http://jjy.shzxlz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qsx.zhixingplan.top

[S40] C++：查找元素
来源：http://ccw.zhaomingkeji.xyz

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ydm.jqgufenzy.top

[S41] C++：类与构造函数
来源：http://lqz.andypj.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ldn.hcnkem.com

[S42] C++：继承与虚函数
来源：http://ans.uphjek.com

class B : public Base { public: void f() override {} };
来源：http://mdl.sjlbkw.cn

[S43] C++：智能指针
来源：http://scz.svipenyu.cn

auto p = std::make_unique<int>(5);
来源：http://lhl.epnwcf.com

[S44] C++：引用传参
来源：http://ivk.aibaodan.cn

void inc(int &x) { ++x; }
来源：http://cdf.sysykeji.top

[S45] C++：lambda
来源：http://jzv.nanxinkj.top

auto add = [](int a, int b) { return a + b; };
来源：http://zfi.wangdashe.top

[S46] C++：函数模板
来源：http://syx.jiagoushi.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cop.yj20258888.top

[S47] C++：结构化绑定遍历
来源：http://cfy.ctjpmb.com

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dfu.cheryme.top

[S48] C++：逐行读文件
来源：http://gli.ywan-chungtsiang.top

std::ifstream in("a.txt");  std::string line;
来源：http://mpe.zhijiandao.cn

while (std::getline(in, line)) { }
来源：http://rzz.jqgufenzy.top

[S49] C++：写文件
来源：http://vpm.yangfankeji.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vln.yuanzhike.top

[S50] C++：格式化数字
来源：http://lnu.uphjek.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://moy.cqqwz.cn

[S51] C++：显式类型转换
来源：http://pqf.haohaochexian.top

static_cast<double>(a) / b
来源：http://epb.hcnkem.com

[S52] C++：const 与 noexcept
来源：http://xpv.wangdashe.top

int size() const noexcept { return n_; }
来源：http://ifc.zdbjq.cn

[S53] C++：移动语义
来源：http://ojf.zhoulong.xyz

std::vector<int> w = std::move(v);
来源：http://dvs.snrcjt.cn

[S54] C++：异常处理
来源：http://fcm.sweek.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ywv.jyoumei.cn

[S55] C++：结构化绑定
来源：http://nza.epnwcf.com

auto [a, b] = std::make_pair(1, 2);
来源：http://pbs.yj20258.top

[S56] C++：optional
来源：http://sit.yj20258.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yra.cqqwz.cn

[S57] C++：编译期常量
来源：http://biv.jiagoushi.top

constexpr int N = 10;
来源：http://ved.gotoacloud.top

[S58] C++：命名空间
来源：http://nkt.zhixingplan.top

namespace ns { int f() { return 1; } }
来源：http://rpo.zdbjq.cn

[S59] C++：静态断言
来源：http://mrj.feifeiyinyue.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zsd.jinqigufen.top

[S60] C++：遍历并删除元素
来源：http://hfq.yuanzhike.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ena.yvedp.cn

================================================================================
来源：http://iqw.yuxming.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ymr.cqqwz.cn

================================================================================
来源：http://sbm.aizwys.cn

[T01] Kotlin：Hello World
来源：http://jco.yanxiufei.cn

println("Hello")
来源：http://igg.zhaomingkeji.xyz

[T02] Kotlin：变量
来源：http://zlu.cucudq.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iay.jiagoushi.top

[T03] Kotlin：字符串模板
来源：http://gbp.ehwqpu.com

"值: $b"
来源：http://pus.hfpthk.cn

[T04] Kotlin：空安全
来源：http://ies.birdmap.top

val n: String? = null;  n?.length
来源：http://xjw.svipenyu.cn


<!-- 参考信息 -->