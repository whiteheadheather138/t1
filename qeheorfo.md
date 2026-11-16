代发 wailian999

name="${1:-default}"
来源：http://thg.sufxvd.cn

[R06] 判断命令是否存在
来源：http://ehn.tarul.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://utv.tarul.cn

[R07] if 判断文件
来源：http://eeu.jyoumei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jic.jinqigufen.top

[R08] 数值比较
来源：http://uyt.meibo888.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rov.zhoulong.xyz

[R09] 字符串比较
来源：http://qsw.ydzc1.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mzs.jinqigufen.top

[R10] 正则匹配
来源：http://zfz.wangshuangyany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ojo.shanyushiyangtech.top

[R11] case 多分支
来源：http://xkz.fengsongda.top

case "$1" in
来源：http://stu.ybcxt.top

start) echo "启动" ;;
来源：http://qpl.kuanghao11.cn

stop)  echo "停止" ;;
来源：http://xut.tianlin.xyz

*)     echo "未知命令" ;;
来源：http://syi.zhixingplan.top

esac
来源：http://gtd.zycfv.cn

[R12] for 遍历文件
来源：http://jox.meibo888.top

for f in *.txt; do echo "$f"; done
来源：http://uma.aibaodan.cn

[R13] for 计数循环
来源：http://bdv.haohaochexian.top

for i in {1..10}; do echo "$i"; done
来源：http://jqr.jyoumei.cn

[R14] C 风格 for
来源：http://amf.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://opv.meibo888.top

[R15] while 逐行读文件
来源：http://koz.xylfe.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://iiz.hcnkem.com

[R16] until 等待条件
来源：http://hmb.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zlb.dianchejie.cn

[R17] 数组定义与取值
来源：http://xkq.fehbvm.com

arr=(a b c); echo "${arr[0]}"
来源：http://frb.fzhhl.top

[R18] 遍历数组
来源：http://orl.uphjek.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://udm.yanxiufei.cn

[R19] 数组长度
来源：http://zfc.jinyuanbaomall.cn

echo "${#arr[@]}"
来源：http://htc.yuanzhike.top

[R20] 关联数组（字典）
来源：http://rwu.yongpay.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dko.smart0.xyz

[R21] 字符串长度
来源：http://gzx.iojbl.cn

echo "${#s}"
来源：http://lym.tianlin.xyz

[R22] 截取子串
来源：http://wre.fktsv.cn

echo "${s:0:5}"
来源：http://dus.tarul.cn

[R23] 字符串替换
来源：http://lta.jyoumei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dwt.zhoulong.xyz

[R24] 大小写转换
来源：http://gcb.xylfe.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jnm.yonumen.top

[R25] 去后缀 / 去前缀
来源：http://eyv.zdqjudy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://tsz.xuanzx.com

[R26] 命令替换
来源：http://whx.gotoacloud.top

now=$(date +%F); echo "$now"
来源：http://gli.xziqi.cn

[R27] 算术展开
来源：http://ned.hammf.cn

echo $((1 + 2 * 3))
来源：http://szz.sjlbkw.cn

[R28] 浮点运算
来源：http://ttd.chenjidiqi.icu

echo "scale=2; 10/3" | bc
来源：http://qyd.svipenyu.cn

[R29] 定义函数
来源：http://phq.zhongyouzk.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ego.pengpengdd.cyou

[R30] 函数返回状态码
来源：http://evq.yj20258.top

f() { return 0; }; f || echo "失败了"
来源：http://fyv.sysykeji.top

[R31] 局部变量
来源：http://bjk.sxryk.cn

f() { local x=1; echo "$x"; }
来源：http://oya.zycfv.cn

[R32] 参数个数校验
来源：http://ovx.ehwqpu.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rwr.svipenyu.cn

[R33] 捕获错误并提示行号
来源：http://lyw.gaohongyu789.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://olt.aizwys.cn

[R34] 退出时清理
来源：http://wrq.jinqigufen.top

trap 'rm -f "$tmp"' EXIT
来源：http://ngf.shuidangran.top

[R35] 后台执行并等待
来源：http://wkr.316326.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://wms.hongshengwenyu.top

[R36] 并发执行多个任务
来源：http://xxd.zdbjq.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qwx.ywan-chungtsiang.top

[R37] 把输出赋给变量
来源：http://jxn.vehdjk.com

files=$(ls -1)
来源：http://khp.zhengqikj.top

[R38] 管道串联
来源：http://jci.yuanzhike.top

cat a.txt | grep -i error | wc -l
来源：http://cit.jyoumei.cn

[R39] 重定向标准输出与错误
来源：http://bso.cqqwz.cn

cmd > out.log 2>&1
来源：http://jnp.nanxinkj.top

[R40] 追加写日志
来源：http://whz.nwbrower.top

echo "log" >> out.log
来源：http://rky.epnwcf.com

[R41] 丢弃输出
来源：http://cqj.jinqigfzy.top

cmd >/dev/null 2>&1
来源：http://ych.cqqwz.cn

[R42] 输入重定向
来源：http://ctf.hcnkem.com

wc -l < a.txt
来源：http://cyt.hysaishi.cn

[R43] 按名字查找文件
来源：http://uzb.yuanzhike.top

find . -name "*.log" -type f
来源：http://sbh.yuxming.cn

[R44] 按修改时间查找
来源：http://uvz.guannengcc.top

find . -mtime -7 -type f
来源：http://gka.yuanzhike.top

[R45] 批量删除
来源：http://ccj.zhongyouzk.top

find . -name "*.tmp" -delete
来源：http://uaa.smart0.xyz

[R46] 递归替换文件内容
来源：http://cah.tanke756.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vxl.gotoacloud.top

[R47] sed 单行替换
来源：http://lsw.yangfankeji.com

sed -i 's/foo/bar/g' a.txt
来源：http://bvy.tian-w.cn

[R48] awk 取指定列
来源：http://ftr.ywan-chungtsiang.top

awk '{print $1, $3}' a.txt
来源：http://nez.haohaochexian.top

[R49] awk 带条件
来源：http://edp.shanyushiyangtech.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nav.birdmap.top

[R50] awk 求和
来源：http://mxe.gzhubu.top

awk '{s += $2} END {print s}' a.txt
来源：http://npi.jlsjyb.cn

[R51] 排序去重取前几
来源：http://wyf.epnwcf.com

sort a.txt | uniq -c | sort -rn | head
来源：http://yez.iojbl.cn

[R52] 统计行数
来源：http://edz.vqdsnc.cn

wc -l a.txt
来源：http://zve.meibo888.top

[R53] 查看文件头与实时尾
来源：http://yro.guannengcc.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://agh.gaohongyu789.top

[R54] 比较两个文件
来源：http://fjt.cdnleiting.top

diff a.txt b.txt
来源：http://lql.iojbl.cn

[R55] 压缩与解压
来源：http://ylg.pycfn.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jmc.hfpthk.cn

[R56] 远程拷贝
来源：http://gcv.zhijiandao.cn

scp file user@host:/path/
来源：http://fyo.tianlin.xyz

[R57] 远程执行命令
来源：http://zfz.zycfv.cn

ssh user@host 'uptime'
来源：http://njy.zhongyouzk.top

[R58] 下载文件
来源：http://hqn.cqqwz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://upw.yj20258888.top

[R59] 发 POST JSON
来源：http://vty.sufxvd.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://trs.nwbrower.top

[R60] 只看 HTTP 状态码
来源：http://oak.haohaochexian.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tqh.shanyushiyangtech.top

[R61] 磁盘占用
来源：http://kec.jinqigfzy.top

df -h;  du -sh *
来源：http://mur.zycfv.cn

[R62] 找最占空间的文件
来源：http://jeo.gaohongyu789.top

du -ah . | sort -rh | head -10
来源：http://doq.ywan-chungtsiang.top

[R63] 内存与进程
来源：http://pzs.snrcjt.cn

free -h;  ps aux | grep nginx
来源：http://tpe.yuxming.cn

[R64] 结束进程
来源：http://nbx.zhiwuduotai.top

kill -9 $(pgrep -f app.py)
来源：http://jrb.gaohongyu789.top

[R65] 查看端口占用
来源：http://ihm.jianghu66.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uvu.snrcjt.cn

[R66] 定时任务
来源：http://uvn.shuidangran.top

crontab -e;  crontab -l
来源：http://cpg.snrcjt.cn

[R67] 生成随机十六进制串
来源：http://chp.quarkkingdee.top

openssl rand -hex 16
来源：http://ivf.gzhubu.top

[R68] 计算文件校验值
来源：http://yrw.chenlongwang.top

sha256sum a.txt;  md5sum a.txt
来源：http://nve.havefunace.top

[R69] 生成随机密码
来源：http://qsl.xinyue.icu

head -c 16 /dev/urandom | base64
来源：http://wdb.shangyingyoupin.top

[R70] 时间戳与互转
来源：http://oxh.hnqzz.top

date +%s;  date -d @1700000000
来源：http://heq.sysykeji.top

[R71] 日期格式化
来源：http://egj.fktsv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bbw.sweek.top

[R72] 等待端口就绪
来源：http://zun.yueranfly.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yes.tian-w.cn

[R73] 分割大日志
来源：http://hsn.fktsv.cn

split -l 1000 big.log part_
来源：http://xas.feifeiyinyue.top

[R74] 批量重命名
来源：http://xpw.chenzaomai.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fum.yuanzhike.top

[R75] 导出环境变量
来源：http://lbp.sxryk.cn

export PATH="$HOME/bin:$PATH"
来源：http://bsm.shzxlz.cn

[R76] 使用临时文件
来源：http://hur.nwbrower.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ixo.zhiwuduotai.top

[R77] 读取用户输入
来源：http://anu.hnxiangtu.top

read -rp "请输入: " ans
来源：http://xks.shzxlz.cn

[R78] 交互式菜单
来源：http://exb.chenlongwang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zfp.haohaochexian.top

[R79] 解析命令行选项
来源：http://epx.epnwcf.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qdn.yj20258.top

[R80] 查看脚本执行耗时
来源：http://ecu.iojbl.cn

time ./run.sh
来源：http://nxx.cdnleiting.top

================================================================================
来源：http://hrd.pycfn.com

S. C / C++ 专题
来源：http://mfk.hesvh.cn

================================================================================
来源：http://nmr.tanke756.top

[S01] C：Hello World
来源：http://ciq.zhijiandao.cn

#include <stdio.h>
来源：http://qyb.gzhubu.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ezi.fzhhl.top

[S02] C：变量与格式化输出
来源：http://dwk.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://fui.hfpthk.cn

[S03] C：读入整数
来源：http://rue.xingfuxueyuan.xyz

int x; scanf("%d", &x);
来源：http://orw.wangdashe.top

[S04] C：字符串复制
来源：http://aac.yvedp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://afr.shuidangran.top

[S05] C：字符串长度
来源：http://loi.yj20258888.top

strlen(s)
来源：http://lcv.bbcook.cn

[S06] C：字符串比较
来源：http://mxr.gzhubu.top

strcmp(a, b) == 0
来源：http://zmm.jiagoushi.top

[S07] C：数组遍历求和
来源：http://lih.zycfv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bbc.gzhubu.top

[S08] C：动态内存分配与释放
来源：http://kva.yuanzhike.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://exg.hnxiangtu.top

[S09] C：结构体定义与初始化
来源：http://uim.zdqjudy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pdq.jlsjyb.cn

[S10] C：指针与解引用
来源：http://eli.jlsjyb.cn

int *p = &a;  *p = 5;
来源：http://ecy.xingfuxueyuan.xyz

[S11] C：逐行读文件
来源：http://hmz.xylfe.cn

FILE *f = fopen("a.txt", "r");
来源：http://ywo.sysykeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ful.shanyushiyangtech.top

fclose(f);
来源：http://mof.snrcjt.cn

[S12] C：写文件
来源：http://igr.dianchejie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://std.sxryk.cn

[S13] C：宏定义
来源：http://nvu.uphjek.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ncq.jinqigfzy.top

[S14] C：枚举
来源：http://zil.yonumen.top

enum Color { RED, GREEN, BLUE };
来源：http://jkb.ydzc1.top

[S15] C：类型转换
来源：http://pfz.jinqigfzy.top

(double) a / b
来源：http://cpl.iojbl.cn

[S16] C：位操作置位
来源：http://mwh.kuanghao11.cn

x |= (1 << 3);
来源：http://rbe.yonumen.top

[S17] C：安全拼接字符串
来源：http://qle.tarul.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fch.sxryk.cn

[S18] C：命令行参数
来源：http://xkk.epnwcf.com

int main(int argc, char **argv)
来源：http://qit.pycfn.com

[S19] C：快速排序
来源：http://sry.yuxming.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mgq.iojbl.cn

[S20] C：二分查找
来源：http://qaa.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xum.nwbrower.top

[S21] C：字符类别判断
来源：http://avu.zhijiandao.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fns.yj20258888.top

[S22] C：字符串转数字
来源：http://kdy.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://qbj.hesvh.cn

[S23] C：随机数
来源：http://gyv.tarul.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mjc.jyoumei.cn

[S24] C：获取本地时间
来源：http://uuk.chenlongwang.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://xoa.andypj.xyz

[S25] C：内存拷贝
来源：http://mys.shanyushiyangkeji.top

memcpy(dst, src, n);
来源：http://spy.hnqzz.top

[S26] C：内存清零
来源：http://uzn.iojbl.cn

memset(a, 0, sizeof a);
来源：http://vfu.jinghuilouyu.cn

[S27] C：定义常量
来源：http://cef.fanxiaobao.xyz

const double PI = 3.14159;
来源：http://mcz.zhoulong.xyz

[S28] C：静态变量
来源：http://aoi.bbcook.cn

static int counter = 0;
来源：http://vqq.cucudq.cn

[S29] C：变参函数
来源：http://eke.jqgufenzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zqq.ivvv.top

[S30] C：头文件保护
来源：http://lwe.hcnkem.com

#ifndef X_H
来源：http://pgr.ehwqpu.com

#define X_H
来源：http://tcz.ehwqpu.com

#endif
来源：http://xnz.0kj1m.cn

[S31] C++：Hello World
来源：http://jfh.jinqigufen.top

#include <iostream>
来源：http://rcg.epnwcf.com

int main() { std::cout << "Hello\n"; }
来源：http://twc.hfpthk.cn

[S32] C++：字符串
来源：http://hpo.haohaochexian.top

std::string s = "hi";  s += "!";
来源：http://ufp.smart0.xyz

[S33] C++：vector 增删
来源：http://tzt.zhongyouzk.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qjw.hywenlv.cn

[S34] C++：遍历 vector
来源：http://cwk.chenzaomai.com

for (auto &x : v) { std::cout << x; }
来源：http://ukw.jinyuanbaomall.cn

[S35] C++：map
来源：http://eha.nanxinkj.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vlm.zhoulong.xyz

[S36] C++：unordered_map
来源：http://nuw.bbcook.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xpq.daxiang520.top

[S37] C++：set
来源：http://haz.shuidangran.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rhm.chenlongwang.top

[S38] C++：排序
来源：http://cvw.hnxiangtu.top

std::sort(v.begin(), v.end());
来源：http://eqc.quarkkingdee.top

[S39] C++：自定义比较器排序
来源：http://zvu.hysaishi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://alo.tianlin.xyz

[S40] C++：查找元素
来源：http://bbe.xylfe.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ikm.cdnleiting.top

[S41] C++：类与构造函数
来源：http://yjk.yj202588.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qkf.fanxiaobao.xyz

[S42] C++：继承与虚函数
来源：http://ncs.bjfxy.top

class B : public Base { public: void f() override {} };
来源：http://lcd.gzhubu.top

[S43] C++：智能指针
来源：http://tih.ehwqpu.com

auto p = std::make_unique<int>(5);
来源：http://esj.ivvv.top

[S44] C++：引用传参
来源：http://jcg.fehbvm.com

void inc(int &x) { ++x; }
来源：http://jfx.chenjidiqi.icu

[S45] C++：lambda
来源：http://rez.wangdashe.top

auto add = [](int a, int b) { return a + b; };
来源：http://sez.vqdsnc.cn

[S46] C++：函数模板
来源：http://ttr.ydjk.org.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yjf.guowangkeji.top

[S47] C++：结构化绑定遍历
来源：http://esq.cheryme.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ibw.bjfxy.top

[S48] C++：逐行读文件
来源：http://gtg.jinyuanbaomall.cn

std::ifstream in("a.txt");  std::string line;
来源：http://phz.iojbl.cn

while (std::getline(in, line)) { }
来源：http://xtb.redwolf501.top

[S49] C++：写文件
来源：http://iyb.chenjidiqi.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://afl.guowangkeji.top

[S50] C++：格式化数字
来源：http://nkd.shanyushiyangkeji.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cgi.mhx1999.top

[S51] C++：显式类型转换
来源：http://iip.fengsongda.top

static_cast<double>(a) / b
来源：http://nsv.havefunace.top

[S52] C++：const 与 noexcept
来源：http://uii.ydzc1.top

int size() const noexcept { return n_; }
来源：http://kbs.hfpthk.cn

[S53] C++：移动语义
来源：http://thh.hesvh.cn

std::vector<int> w = std::move(v);
来源：http://kbc.gaohongyu789.top

[S54] C++：异常处理
来源：http://kmo.andypj.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jqe.chenjidiqi.icu

[S55] C++：结构化绑定
来源：http://vhm.fehbvm.com

auto [a, b] = std::make_pair(1, 2);
来源：http://agz.hywenlv.cn

[S56] C++：optional
来源：http://sbc.cheryme.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pmq.gogol.net.cn

[S57] C++：编译期常量
来源：http://qva.bjfxy.top

constexpr int N = 10;
来源：http://rvr.nanxuanxn.top

[S58] C++：命名空间
来源：http://cev.ywan-chungtsiang.top

namespace ns { int f() { return 1; } }
来源：http://thq.ivvv.top

[S59] C++：静态断言
来源：http://fab.svipenyu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xpn.jinyuanbaomall.cn

[S60] C++：遍历并删除元素
来源：http://iye.gzhubu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tfl.jinqigufen.top

================================================================================
来源：http://izo.hnxiangtu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fsm.guannengcc.top

================================================================================
来源：http://ddn.hnqzz.top

[T01] Kotlin：Hello World
来源：http://spc.jinghuilouyu.cn

println("Hello")
来源：http://sfr.jianghu66.top

[T02] Kotlin：变量
来源：http://izi.vqdsnc.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xwx.bjfxy.top

[T03] Kotlin：字符串模板
来源：http://rzn.snrcjt.cn

"值: $b"
来源：http://muy.jyoumei.cn

[T04] Kotlin：空安全
来源：http://qkp.yonumen.top

val n: String? = null;  n?.length
来源：http://iss.jiagoushi.top

[T05] Kotlin：when 表达式
来源：http://iqa.bbcook.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://isb.zhongyouzk.top

[T06] Kotlin：集合映射
来源：http://qof.fehbvm.com

listOf(1, 2, 3).map { it * 2 }
来源：http://znw.hywenlv.cn


<!-- 参考信息 -->