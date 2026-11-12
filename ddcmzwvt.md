代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://emg.ehwqpu.com

[R08] 数值比较
来源：http://scl.yongpay.top

if (( a > b )); then echo "a 更大"; fi
来源：http://jdw.mhx1999.top

[R09] 字符串比较
来源：http://yzz.wangshuangyany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gdr.andypj.xyz

[R10] 正则匹配
来源：http://kmx.jinyuanbaomall.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rtj.fzhhl.top

[R11] case 多分支
来源：http://uii.hammf.cn

case "$1" in
来源：http://qqd.xuetiantiany.cn

start) echo "启动" ;;
来源：http://whf.vehdjk.com

stop)  echo "停止" ;;
来源：http://lqo.shangyingyoupin.top

*)     echo "未知命令" ;;
来源：http://xxf.sufxvd.cn

esac
来源：http://voh.yonumen.top

[R12] for 遍历文件
来源：http://ytb.chenlongwang.top

for f in *.txt; do echo "$f"; done
来源：http://uvv.ppjwa.cn

[R13] for 计数循环
来源：http://nda.havefunace.top

for i in {1..10}; do echo "$i"; done
来源：http://erb.hfpthk.cn

[R14] C 风格 for
来源：http://xtj.yueranfly.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xgy.xziqi.cn

[R15] while 逐行读文件
来源：http://zxb.jinqigfzy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wsc.cucudq.cn

[R16] until 等待条件
来源：http://yip.sxryk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ajo.shzxlz.cn

[R17] 数组定义与取值
来源：http://zot.yonumen.top

arr=(a b c); echo "${arr[0]}"
来源：http://ahk.shzxlz.cn

[R18] 遍历数组
来源：http://awc.yueranfly.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nri.cdnleiting.top

[R19] 数组长度
来源：http://mvt.guowangkeji.top

echo "${#arr[@]}"
来源：http://chh.yanxiufei.cn

[R20] 关联数组（字典）
来源：http://suv.epnwcf.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fmr.jlsjyb.cn

[R21] 字符串长度
来源：http://hty.shanyushiyangtech.top

echo "${#s}"
来源：http://gsa.yanxiufei.cn

[R22] 截取子串
来源：http://idb.tianlin.xyz

echo "${s:0:5}"
来源：http://qsr.zdqjudy.top

[R23] 字符串替换
来源：http://cij.vehdjk.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mqi.yanxiufei.cn

[R24] 大小写转换
来源：http://jgw.feifeiyinyue.top

echo "${s^^}"; echo "${s,,}"
来源：http://rsd.xziqi.cn

[R25] 去后缀 / 去前缀
来源：http://pkm.xylfe.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://itf.yanxiufei.cn

[R26] 命令替换
来源：http://pxp.mhx1999.top

now=$(date +%F); echo "$now"
来源：http://ocf.zhiwuduotai.top

[R27] 算术展开
来源：http://rsw.shanyushiyangkeji.top

echo $((1 + 2 * 3))
来源：http://tvm.gzhubu.top

[R28] 浮点运算
来源：http://bfl.nanxuanxn.top

echo "scale=2; 10/3" | bc
来源：http://zvb.ydzc1.top

[R29] 定义函数
来源：http://rfz.zycfv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://byk.meibo888.top

[R30] 函数返回状态码
来源：http://rwf.shzxlz.cn

f() { return 0; }; f || echo "失败了"
来源：http://hnb.daria6918.cn

[R31] 局部变量
来源：http://dem.cashguo.top

f() { local x=1; echo "$x"; }
来源：http://nwy.hesvh.cn

[R32] 参数个数校验
来源：http://vtr.zdbjq.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lrd.cucudq.cn

[R33] 捕获错误并提示行号
来源：http://ckj.feifeiyinyue.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qte.cheryme.top

[R34] 退出时清理
来源：http://gtf.cheryme.top

trap 'rm -f "$tmp"' EXIT
来源：http://xmh.nanxinkj.top

[R35] 后台执行并等待
来源：http://zzn.cheryme.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dwo.jqgufenzy.top

[R36] 并发执行多个任务
来源：http://kgv.tarul.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ksp.gzhubu.top

[R37] 把输出赋给变量
来源：http://maw.chenzaomai.com

files=$(ls -1)
来源：http://mhr.cheryme.top

[R38] 管道串联
来源：http://lsx.wangshuangyany.cn

cat a.txt | grep -i error | wc -l
来源：http://yzl.daxiang520.top

[R39] 重定向标准输出与错误
来源：http://szo.xinyue.icu

cmd > out.log 2>&1
来源：http://ugj.bbcook.cn

[R40] 追加写日志
来源：http://pei.yuanzhike.top

echo "log" >> out.log
来源：http://gmg.jlsjyb.cn

[R41] 丢弃输出
来源：http://foh.jianghu66.top

cmd >/dev/null 2>&1
来源：http://wvz.cqqwz.cn

[R42] 输入重定向
来源：http://lvw.wangshuangyany.cn

wc -l < a.txt
来源：http://tmi.xuetiantiany.cn

[R43] 按名字查找文件
来源：http://nfl.yj20258888.top

find . -name "*.log" -type f
来源：http://jfs.aibaodan.cn

[R44] 按修改时间查找
来源：http://pcr.sjlbkw.cn

find . -mtime -7 -type f
来源：http://igg.xinyue.icu

[R45] 批量删除
来源：http://vvx.vehdjk.com

find . -name "*.tmp" -delete
来源：http://qol.316326.xyz

[R46] 递归替换文件内容
来源：http://pjv.jianghu66.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cdi.pengpengdd.cyou

[R47] sed 单行替换
来源：http://stg.hesvh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://xkh.jyoumei.cn

[R48] awk 取指定列
来源：http://pzt.chenzaomai.com

awk '{print $1, $3}' a.txt
来源：http://xfc.cdnleiting.top

[R49] awk 带条件
来源：http://pvw.cdnleiting.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fcm.yuanzhike.top

[R50] awk 求和
来源：http://ebm.shzxlz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://wda.zdbjq.cn

[R51] 排序去重取前几
来源：http://szp.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lgk.sysykeji.top

[R52] 统计行数
来源：http://zjl.yuxming.cn

wc -l a.txt
来源：http://wkl.fanxiaobao.xyz

[R53] 查看文件头与实时尾
来源：http://wnx.aibaodan.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ypk.andypj.xyz

[R54] 比较两个文件
来源：http://hrn.yj20258888.top

diff a.txt b.txt
来源：http://mdb.yfazqb.com

[R55] 压缩与解压
来源：http://hgm.zycfv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ojg.andypj.xyz

[R56] 远程拷贝
来源：http://xcu.kuanghao11.cn

scp file user@host:/path/
来源：http://cll.cqqwz.cn

[R57] 远程执行命令
来源：http://rtd.xuanzx.com

ssh user@host 'uptime'
来源：http://tlv.meibo888.top

[R58] 下载文件
来源：http://xur.vehdjk.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dpu.guowangkeji.top

[R59] 发 POST JSON
来源：http://ngl.daria6918.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://opj.tian-w.cn

[R60] 只看 HTTP 状态码
来源：http://ika.zhoulong.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dde.sxryk.cn

[R61] 磁盘占用
来源：http://ogm.gzhubu.top

df -h;  du -sh *
来源：http://fej.wangshuangyany.cn

[R62] 找最占空间的文件
来源：http://cio.dashuyun.cn

du -ah . | sort -rh | head -10
来源：http://fnl.yvedp.cn

[R63] 内存与进程
来源：http://jog.pengpengdd.cyou

free -h;  ps aux | grep nginx
来源：http://erd.pengpengdd.cyou

[R64] 结束进程
来源：http://fzf.yueranfly.top

kill -9 $(pgrep -f app.py)
来源：http://xom.ydjk.org.cn

[R65] 查看端口占用
来源：http://usc.fehbvm.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ifg.xylfe.cn

[R66] 定时任务
来源：http://jmc.tian-w.cn

crontab -e;  crontab -l
来源：http://oss.shangyingyoupin.top

[R67] 生成随机十六进制串
来源：http://ivr.gzhubu.top

openssl rand -hex 16
来源：http://xyu.jinyuanbaomall.cn

[R68] 计算文件校验值
来源：http://ydw.tanke756.top

sha256sum a.txt;  md5sum a.txt
来源：http://dyl.xuetiantiany.cn

[R69] 生成随机密码
来源：http://oqq.pycfn.com

head -c 16 /dev/urandom | base64
来源：http://ptj.gaohongyu789.top

[R70] 时间戳与互转
来源：http://gml.hfpthk.cn

date +%s;  date -d @1700000000
来源：http://jrk.xinyue.icu

[R71] 日期格式化
来源：http://vzf.zdbjq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nfd.9152youxi.cn

[R72] 等待端口就绪
来源：http://art.yfazqb.com

until nc -z localhost 3306; do sleep 1; done
来源：http://tvd.hysaishi.cn

[R73] 分割大日志
来源：http://azz.vehdjk.com

split -l 1000 big.log part_
来源：http://jqq.zhoulong.xyz

[R74] 批量重命名
来源：http://dqy.cucudq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dpn.dashuyun.cn

[R75] 导出环境变量
来源：http://qha.shuidangran.top

export PATH="$HOME/bin:$PATH"
来源：http://cbr.meibo888.top

[R76] 使用临时文件
来源：http://lwg.vehdjk.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cdv.hesvh.cn

[R77] 读取用户输入
来源：http://gsc.ppjwa.cn

read -rp "请输入: " ans
来源：http://cyd.ppjwa.cn

[R78] 交互式菜单
来源：http://xcs.zhaomingkeji.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://uzl.cdnleiting.top

[R79] 解析命令行选项
来源：http://aub.xuetiantiany.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fvo.yanxiufei.cn

[R80] 查看脚本执行耗时
来源：http://hdj.cheryme.top

time ./run.sh
来源：http://plm.xuetiantiany.cn

================================================================================
来源：http://nsm.dashuyun.cn

S. C / C++ 专题
来源：http://fik.yuanzhike.top

================================================================================
来源：http://wvz.birdmap.top

[S01] C：Hello World
来源：http://wvr.dianchejie.cn

#include <stdio.h>
来源：http://thn.yanxiufei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://vfj.hysaishi.cn

[S02] C：变量与格式化输出
来源：http://zjk.xingfuxueyuan.xyz

int a = 10; printf("%d\n", a);
来源：http://ncv.sweek.top

[S03] C：读入整数
来源：http://aij.iojbl.cn

int x; scanf("%d", &x);
来源：http://yow.tarul.cn

[S04] C：字符串复制
来源：http://eeg.mhx1999.top

char dst[32]; strcpy(dst, "hi");
来源：http://qme.wangdashe.top

[S05] C：字符串长度
来源：http://ppa.cheryme.top

strlen(s)
来源：http://kcg.hesvh.cn

[S06] C：字符串比较
来源：http://fuj.kuanghao11.cn

strcmp(a, b) == 0
来源：http://ett.dashuyun.cn

[S07] C：数组遍历求和
来源：http://zwa.hysaishi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cal.tarul.cn

[S08] C：动态内存分配与释放
来源：http://zgq.xylfe.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vkc.gaohongyu789.top

[S09] C：结构体定义与初始化
来源：http://pde.yuanzhike.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://duv.zhaomingkeji.xyz

[S10] C：指针与解引用
来源：http://dvj.ydzc1.top

int *p = &a;  *p = 5;
来源：http://ldn.yvedp.cn

[S11] C：逐行读文件
来源：http://hyu.ydzc1.top

FILE *f = fopen("a.txt", "r");
来源：http://csk.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://kcy.daxiang520.top

fclose(f);
来源：http://mmc.gaohongyu789.top

[S12] C：写文件
来源：http://flh.quarkkingdee.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jpj.yueranfly.top

[S13] C：宏定义
来源：http://urj.fehbvm.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://taz.shzxlz.cn

[S14] C：枚举
来源：http://rrc.xuanzx.com

enum Color { RED, GREEN, BLUE };
来源：http://cfy.svipenyu.cn

[S15] C：类型转换
来源：http://hdt.smart0.xyz

(double) a / b
来源：http://xpi.yj202588.top

[S16] C：位操作置位
来源：http://ctr.wangdashe.top

x |= (1 << 3);
来源：http://pgg.jiagoushi.top

[S17] C：安全拼接字符串
来源：http://sbr.dianchejie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://igs.yvedp.cn

[S18] C：命令行参数
来源：http://vmd.yj20258.top

int main(int argc, char **argv)
来源：http://uoy.chenzaomai.com

[S19] C：快速排序
来源：http://gvd.chenzaomai.com

qsort(a, n, sizeof(int), cmp);
来源：http://awd.xingfuxueyuan.xyz

[S20] C：二分查找
来源：http://dhu.hysaishi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jcn.yj202588.top

[S21] C：字符类别判断
来源：http://tdv.sufxvd.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ryd.fengsongda.top

[S22] C：字符串转数字
来源：http://sbi.ywan-chungtsiang.top

atoi("42");  strtod("3.14", NULL);
来源：http://ack.hnxiangtu.top

[S23] C：随机数
来源：http://izm.meibo888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://xuc.yj20258.top

[S24] C：获取本地时间
来源：http://iln.guannengcc.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kxg.sufxvd.cn

[S25] C：内存拷贝
来源：http://zii.jinyuanbaomall.cn

memcpy(dst, src, n);
来源：http://gei.daria6918.cn

[S26] C：内存清零
来源：http://spv.jqgufenzy.top

memset(a, 0, sizeof a);
来源：http://upw.shanyushiyangtech.top

[S27] C：定义常量
来源：http://moe.c1oappe.top

const double PI = 3.14159;
来源：http://twe.jqgfzy.top

[S28] C：静态变量
来源：http://zcj.tian-w.cn

static int counter = 0;
来源：http://wkf.ybcxt.top

[S29] C：变参函数
来源：http://row.uphjek.com

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xky.shuidangran.top

[S30] C：头文件保护
来源：http://ocq.ydzc1.top

#ifndef X_H
来源：http://zzz.wangshuangyany.cn

#define X_H
来源：http://wza.yj20258.top

#endif
来源：http://zga.gzhubu.top

[S31] C++：Hello World
来源：http://ujd.hcnkem.com

#include <iostream>
来源：http://kyy.52xcode.cn

int main() { std::cout << "Hello\n"; }
来源：http://vux.zhijiandao.cn

[S32] C++：字符串
来源：http://fvn.shzxlz.cn

std::string s = "hi";  s += "!";
来源：http://hwu.mhx1999.top

[S33] C++：vector 增删
来源：http://bsj.zhijiandao.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ang.hnxiangtu.top

[S34] C++：遍历 vector
来源：http://ewq.chenzaomai.com

for (auto &x : v) { std::cout << x; }
来源：http://sjx.feifeiyinyue.top

[S35] C++：map
来源：http://xah.haohaochexian.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ark.c1oappe.top

[S36] C++：unordered_map
来源：http://kwg.yongpay.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xaw.daxiang520.top

[S37] C++：set
来源：http://kfa.9152youxi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qiq.sysykeji.top

[S38] C++：排序
来源：http://phi.epnwcf.com

std::sort(v.begin(), v.end());
来源：http://for.haohaochexian.top

[S39] C++：自定义比较器排序
来源：http://iwn.yongpay.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lcn.dianchejie.cn

[S40] C++：查找元素
来源：http://oeo.hesvh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://awy.fengsongda.top

[S41] C++：类与构造函数
来源：http://pvr.zdqjudy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zvb.fengsongda.top

[S42] C++：继承与虚函数
来源：http://adl.yj202588.top

class B : public Base { public: void f() override {} };
来源：http://tqr.zhoulong.xyz

[S43] C++：智能指针
来源：http://zaj.shzxlz.cn

auto p = std::make_unique<int>(5);
来源：http://huc.0kj1m.cn

[S44] C++：引用传参
来源：http://xtl.fktsv.cn

void inc(int &x) { ++x; }
来源：http://kpk.daxiang520.top

[S45] C++：lambda
来源：http://lnr.yfazqb.com

auto add = [](int a, int b) { return a + b; };
来源：http://gtq.cdnleiting.top

[S46] C++：函数模板
来源：http://lke.quarkkingdee.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://asr.tanke756.top

[S47] C++：结构化绑定遍历
来源：http://kkn.hammf.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iku.yonumen.top

[S48] C++：逐行读文件
来源：http://shz.sjlbkw.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gzi.birdmap.top

while (std::getline(in, line)) { }
来源：http://qni.xingfuxueyuan.xyz

[S49] C++：写文件
来源：http://nsi.chenjidiqi.icu

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bzx.tanke756.top

[S50] C++：格式化数字
来源：http://avd.daria6918.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://plp.redwolf501.top

[S51] C++：显式类型转换
来源：http://vnz.jyoumei.cn

static_cast<double>(a) / b
来源：http://svw.shanyushiyangkeji.top

[S52] C++：const 与 noexcept
来源：http://jou.yueranfly.top

int size() const noexcept { return n_; }
来源：http://iqq.gotoacloud.top

[S53] C++：移动语义
来源：http://snu.zhiwuduotai.top

std::vector<int> w = std::move(v);
来源：http://axh.meibo888.top

[S54] C++：异常处理
来源：http://mii.ybcxt.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fac.hysaishi.cn

[S55] C++：结构化绑定
来源：http://kgh.meibo888.top

auto [a, b] = std::make_pair(1, 2);
来源：http://axi.fehbvm.com

[S56] C++：optional
来源：http://oku.zhiwuduotai.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bxg.tarul.cn

[S57] C++：编译期常量
来源：http://vkd.cucudq.cn

constexpr int N = 10;
来源：http://avg.ybcxt.top

[S58] C++：命名空间
来源：http://gqk.gaohongyu789.top

namespace ns { int f() { return 1; } }
来源：http://pve.gaohongyu789.top

[S59] C++：静态断言
来源：http://wkg.daxiang520.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wkc.fktsv.cn

[S60] C++：遍历并删除元素
来源：http://pis.jianghu66.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://poc.xuetiantiany.cn

================================================================================
来源：http://yww.gotoacloud.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://noj.jinghuilouyu.cn

================================================================================
来源：http://quk.zdqjudy.top

[T01] Kotlin：Hello World
来源：http://dvx.jiagoushi.top

println("Hello")
来源：http://sqe.meibo888.top

[T02] Kotlin：变量
来源：http://mvq.9152youxi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mvh.gzhubu.top

[T03] Kotlin：字符串模板
来源：http://mes.sxryk.cn

"值: $b"
来源：http://nle.chenzaomai.com

[T04] Kotlin：空安全
来源：http://sxg.zhoulong.xyz

val n: String? = null;  n?.length
来源：http://oph.yanxiufei.cn

[T05] Kotlin：when 表达式
来源：http://dik.hesvh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tig.tarul.cn

[T06] Kotlin：集合映射
来源：http://azx.cdnleiting.top

listOf(1, 2, 3).map { it * 2 }
来源：http://poy.cucudq.cn

[T07] Kotlin：集合过滤
来源：http://ths.cheryme.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://mxx.dianchejie.cn

[T08] Kotlin：数据类
来源：http://yzr.dianchejie.cn

data class User(val name: String, val age: Int)
来源：http://pqc.hnqzz.top


<!-- 参考信息 -->