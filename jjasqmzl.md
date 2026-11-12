代发 wailian999

name="${1:-default}"
来源：http://xns.pycfn.com

[R06] 判断命令是否存在
来源：http://qsq.zdqjudy.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://trg.cucudq.cn

[R07] if 判断文件
来源：http://yqi.smart0.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://llf.nanxuanxn.top

[R08] 数值比较
来源：http://iuv.uphjek.com

if (( a > b )); then echo "a 更大"; fi
来源：http://vzf.hfpthk.cn

[R09] 字符串比较
来源：http://ccy.zhengqikj.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pdr.c1oappe.top

[R10] 正则匹配
来源：http://mti.aibaodan.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gon.zhengqikj.top

[R11] case 多分支
来源：http://zqr.yueranfly.top

case "$1" in
来源：http://ean.guannengcc.top

start) echo "启动" ;;
来源：http://cnh.zhixingplan.top

stop)  echo "停止" ;;
来源：http://rfh.fktsv.cn

*)     echo "未知命令" ;;
来源：http://hae.hesvh.cn

esac
来源：http://ygw.yfazqb.com

[R12] for 遍历文件
来源：http://sgl.snrcjt.cn

for f in *.txt; do echo "$f"; done
来源：http://pft.yj202588.top

[R13] for 计数循环
来源：http://phj.zhongyouzk.top

for i in {1..10}; do echo "$i"; done
来源：http://ngb.mhx1999.top

[R14] C 风格 for
来源：http://sjp.xinyue.icu

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tun.cheryme.top

[R15] while 逐行读文件
来源：http://azk.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xrk.yj20258.top

[R16] until 等待条件
来源：http://ikh.jianghu66.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hkd.jinqigufen.top

[R17] 数组定义与取值
来源：http://rlp.aibaodan.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zoq.pengpengdd.cyou

[R18] 遍历数组
来源：http://yhg.sjlbkw.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dqw.yueranfly.top

[R19] 数组长度
来源：http://cmd.kuanghao11.cn

echo "${#arr[@]}"
来源：http://gdz.meibo888.top

[R20] 关联数组（字典）
来源：http://qsu.zhongyouzk.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jfz.zhijiandao.cn

[R21] 字符串长度
来源：http://uhs.jinqigfzy.top

echo "${#s}"
来源：http://okl.vqdsnc.cn

[R22] 截取子串
来源：http://cln.zhaomingkeji.xyz

echo "${s:0:5}"
来源：http://eqf.guannengcc.top

[R23] 字符串替换
来源：http://rbw.zhongyouzk.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://weq.yj20258.top

[R24] 大小写转换
来源：http://xyh.chenzaomai.com

echo "${s^^}"; echo "${s,,}"
来源：http://jwi.yongpay.top

[R25] 去后缀 / 去前缀
来源：http://sws.pycfn.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://wci.nwbrower.top

[R26] 命令替换
来源：http://mjt.xuanzx.com

now=$(date +%F); echo "$now"
来源：http://sez.316326.xyz

[R27] 算术展开
来源：http://elv.tanke756.top

echo $((1 + 2 * 3))
来源：http://zuy.vqdsnc.cn

[R28] 浮点运算
来源：http://vvm.xziqi.cn

echo "scale=2; 10/3" | bc
来源：http://bzm.shzxlz.cn

[R29] 定义函数
来源：http://sfk.feifeiyinyue.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ihn.yanxiufei.cn

[R30] 函数返回状态码
来源：http://yyh.nwbrower.top

f() { return 0; }; f || echo "失败了"
来源：http://umx.yangfankeji.com

[R31] 局部变量
来源：http://tli.zhongyouzk.top

f() { local x=1; echo "$x"; }
来源：http://hqd.tarul.cn

[R32] 参数个数校验
来源：http://ina.hnqzz.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://cbv.bjfxy.top

[R33] 捕获错误并提示行号
来源：http://wzw.shanyushiyangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://cue.aizwys.cn

[R34] 退出时清理
来源：http://xel.dashuyun.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xsj.dianchejie.cn

[R35] 后台执行并等待
来源：http://uyl.fzhhl.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ipz.zhengqikj.top

[R36] 并发执行多个任务
来源：http://htt.jlsjyb.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://lnu.fehbvm.com

[R37] 把输出赋给变量
来源：http://ctt.sweek.top

files=$(ls -1)
来源：http://eiw.yj20258.top

[R38] 管道串联
来源：http://yrr.quarkkingdee.top

cat a.txt | grep -i error | wc -l
来源：http://gqu.yvedp.cn

[R39] 重定向标准输出与错误
来源：http://eaw.sweek.top

cmd > out.log 2>&1
来源：http://wwx.52xcode.cn

[R40] 追加写日志
来源：http://fnz.shanyushiyangtech.top

echo "log" >> out.log
来源：http://ync.dashuyun.cn

[R41] 丢弃输出
来源：http://lbf.nwbrower.top

cmd >/dev/null 2>&1
来源：http://fnd.tarul.cn

[R42] 输入重定向
来源：http://pgs.hywenlv.cn

wc -l < a.txt
来源：http://qig.daria6918.cn

[R43] 按名字查找文件
来源：http://irp.sufxvd.cn

find . -name "*.log" -type f
来源：http://jas.chenzaomai.com

[R44] 按修改时间查找
来源：http://bip.zhaomingkeji.xyz

find . -mtime -7 -type f
来源：http://gra.zhongyouzk.top

[R45] 批量删除
来源：http://jlv.fehbvm.com

find . -name "*.tmp" -delete
来源：http://kzd.cheryme.top

[R46] 递归替换文件内容
来源：http://xak.birdmap.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://neq.gotoacloud.top

[R47] sed 单行替换
来源：http://vvq.epnwcf.com

sed -i 's/foo/bar/g' a.txt
来源：http://unk.tian-w.cn

[R48] awk 取指定列
来源：http://emw.jlsjyb.cn

awk '{print $1, $3}' a.txt
来源：http://hpf.fzhhl.top

[R49] awk 带条件
来源：http://nsv.nanxuanxn.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wfd.cashguo.top

[R50] awk 求和
来源：http://vws.sysykeji.top

awk '{s += $2} END {print s}' a.txt
来源：http://dtc.sweek.top

[R51] 排序去重取前几
来源：http://bfe.jinqigfzy.top

sort a.txt | uniq -c | sort -rn | head
来源：http://sal.chenzaomai.com

[R52] 统计行数
来源：http://vel.chenjidiqi.icu

wc -l a.txt
来源：http://ljo.feifeiyinyue.top

[R53] 查看文件头与实时尾
来源：http://zyc.shanyushiyangtech.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://raf.daxiang520.top

[R54] 比较两个文件
来源：http://wps.havefunace.top

diff a.txt b.txt
来源：http://iqz.birdmap.top

[R55] 压缩与解压
来源：http://cqu.pycfn.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qkx.cheryme.top

[R56] 远程拷贝
来源：http://kpc.yj202588.top

scp file user@host:/path/
来源：http://but.bjfxy.top

[R57] 远程执行命令
来源：http://ogm.shuidangran.top

ssh user@host 'uptime'
来源：http://kop.shangyingyoupin.top

[R58] 下载文件
来源：http://vmk.quarkkingdee.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pav.hnxiangtu.top

[R59] 发 POST JSON
来源：http://rhg.9152youxi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://syd.zhengqikj.top

[R60] 只看 HTTP 状态码
来源：http://crl.xziqi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wya.gogol.net.cn

[R61] 磁盘占用
来源：http://rxf.9152youxi.cn

df -h;  du -sh *
来源：http://skz.yuxming.cn

[R62] 找最占空间的文件
来源：http://dnz.iojbl.cn

du -ah . | sort -rh | head -10
来源：http://djk.ydjk.org.cn

[R63] 内存与进程
来源：http://qfq.chenlongwang.top

free -h;  ps aux | grep nginx
来源：http://zya.zdqjudy.top

[R64] 结束进程
来源：http://xbq.fehbvm.com

kill -9 $(pgrep -f app.py)
来源：http://jwy.zhiwuduotai.top

[R65] 查看端口占用
来源：http://oez.zhaomingkeji.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mfj.birdmap.top

[R66] 定时任务
来源：http://ist.birdmap.top

crontab -e;  crontab -l
来源：http://zfs.wangdashe.top

[R67] 生成随机十六进制串
来源：http://tqc.shanyushiyangtech.top

openssl rand -hex 16
来源：http://qjq.chenzaomai.com

[R68] 计算文件校验值
来源：http://wxp.sjlbkw.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lem.yvedp.cn

[R69] 生成随机密码
来源：http://jmb.haohaochexian.top

head -c 16 /dev/urandom | base64
来源：http://axk.cdnleiting.top

[R70] 时间戳与互转
来源：http://rgf.hnqzz.top

date +%s;  date -d @1700000000
来源：http://eir.hammf.cn

[R71] 日期格式化
来源：http://gjr.meibo888.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://olp.ivvv.top

[R72] 等待端口就绪
来源：http://ujp.zhengqikj.top

until nc -z localhost 3306; do sleep 1; done
来源：http://evp.uphjek.com

[R73] 分割大日志
来源：http://ipd.gotoacloud.top

split -l 1000 big.log part_
来源：http://avd.zhaomingkeji.xyz

[R74] 批量重命名
来源：http://wvq.zhoulong.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hjq.zhongyouzk.top

[R75] 导出环境变量
来源：http://kpj.xylfe.cn

export PATH="$HOME/bin:$PATH"
来源：http://kmr.ydzc1.top

[R76] 使用临时文件
来源：http://edb.jianghu66.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zwe.sufxvd.cn

[R77] 读取用户输入
来源：http://ggj.jlsjyb.cn

read -rp "请输入: " ans
来源：http://bbq.bbcook.cn

[R78] 交互式菜单
来源：http://ugk.snrcjt.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://eqc.yj20258888.top

[R79] 解析命令行选项
来源：http://uaz.haohaochexian.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eys.xuanzx.com

[R80] 查看脚本执行耗时
来源：http://gni.hesvh.cn

time ./run.sh
来源：http://jps.yvedp.cn

================================================================================
来源：http://zwm.hcnkem.com

S. C / C++ 专题
来源：http://msc.zdbjq.cn

================================================================================
来源：http://qea.yfazqb.com

[S01] C：Hello World
来源：http://xhd.dashuyun.cn

#include <stdio.h>
来源：http://yuu.hammf.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mdn.mhx1999.top

[S02] C：变量与格式化输出
来源：http://hin.zhengqikj.top

int a = 10; printf("%d\n", a);
来源：http://ozw.yuanzhike.top

[S03] C：读入整数
来源：http://cfr.cucudq.cn

int x; scanf("%d", &x);
来源：http://oeb.jianghu66.top

[S04] C：字符串复制
来源：http://rel.xylfe.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ptc.yuxming.cn

[S05] C：字符串长度
来源：http://pnu.sxryk.cn

strlen(s)
来源：http://azp.xuetiantiany.cn

[S06] C：字符串比较
来源：http://rby.yueranfly.top

strcmp(a, b) == 0
来源：http://abn.tian-w.cn

[S07] C：数组遍历求和
来源：http://wyg.sxryk.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vlt.zhengqikj.top

[S08] C：动态内存分配与释放
来源：http://iyn.xinyue.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://som.tianlin.xyz

[S09] C：结构体定义与初始化
来源：http://efp.jinghuilouyu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nuu.zdqjudy.top

[S10] C：指针与解引用
来源：http://rsz.shanyushiyangkeji.top

int *p = &a;  *p = 5;
来源：http://oxg.52xcode.cn

[S11] C：逐行读文件
来源：http://suc.zhengqikj.top

FILE *f = fopen("a.txt", "r");
来源：http://yxt.quarkkingdee.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lbm.xuanzx.com

fclose(f);
来源：http://yma.jinghuilouyu.cn

[S12] C：写文件
来源：http://cjh.fehbvm.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mhq.yvedp.cn

[S13] C：宏定义
来源：http://vtq.ehwqpu.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oyr.yj202588.top

[S14] C：枚举
来源：http://ele.zhiwuduotai.top

enum Color { RED, GREEN, BLUE };
来源：http://etu.gzhubu.top

[S15] C：类型转换
来源：http://wjn.cashguo.top

(double) a / b
来源：http://bph.havefunace.top

[S16] C：位操作置位
来源：http://czd.feifeiyinyue.top

x |= (1 << 3);
来源：http://xwu.nanxinkj.top

[S17] C：安全拼接字符串
来源：http://vfg.fanxiaobao.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xny.ydjk.org.cn

[S18] C：命令行参数
来源：http://dly.daxiang520.top

int main(int argc, char **argv)
来源：http://lsy.yangfankeji.com

[S19] C：快速排序
来源：http://rts.hysaishi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bpp.xziqi.cn

[S20] C：二分查找
来源：http://weg.zhoulong.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ezx.aizwys.cn

[S21] C：字符类别判断
来源：http://nlg.ppjwa.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xnv.ybcxt.top

[S22] C：字符串转数字
来源：http://mvo.hnxiangtu.top

atoi("42");  strtod("3.14", NULL);
来源：http://wva.fehbvm.com

[S23] C：随机数
来源：http://edu.fzhhl.top

srand(time(NULL));  int r = rand() % 100;
来源：http://zjb.vehdjk.com

[S24] C：获取本地时间
来源：http://htq.gaohongyu789.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nyu.gotoacloud.top

[S25] C：内存拷贝
来源：http://vot.yueranfly.top

memcpy(dst, src, n);
来源：http://xfx.redwolf501.top

[S26] C：内存清零
来源：http://yiy.chenlongwang.top

memset(a, 0, sizeof a);
来源：http://qwd.shanyushiyangtech.top

[S27] C：定义常量
来源：http://zyd.chenlongwang.top

const double PI = 3.14159;
来源：http://glu.ydzc1.top

[S28] C：静态变量
来源：http://ufq.hongshengwenyu.top

static int counter = 0;
来源：http://ytl.yonumen.top

[S29] C：变参函数
来源：http://nil.dianchejie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://giv.jianghu66.top

[S30] C：头文件保护
来源：http://xid.ctjpmb.com

#ifndef X_H
来源：http://lef.guannengcc.top

#define X_H
来源：http://dup.pycfn.com

#endif
来源：http://ori.cdnleiting.top

[S31] C++：Hello World
来源：http://ifx.yueranfly.top

#include <iostream>
来源：http://foo.snrcjt.cn

int main() { std::cout << "Hello\n"; }
来源：http://krh.ywan-chungtsiang.top

[S32] C++：字符串
来源：http://dic.yonumen.top

std::string s = "hi";  s += "!";
来源：http://nxf.hcnkem.com

[S33] C++：vector 增删
来源：http://wkl.sufxvd.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pnh.ywan-chungtsiang.top

[S34] C++：遍历 vector
来源：http://qsz.nanxinkj.top

for (auto &x : v) { std::cout << x; }
来源：http://cyj.bjfxy.top

[S35] C++：map
来源：http://xjs.jlsjyb.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://muq.zhijiandao.cn

[S36] C++：unordered_map
来源：http://btt.hongshengwenyu.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jfm.sysykeji.top

[S37] C++：set
来源：http://ouf.gzhubu.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xug.tanke756.top

[S38] C++：排序
来源：http://bsv.chenlongwang.top

std::sort(v.begin(), v.end());
来源：http://nie.guowangkeji.top

[S39] C++：自定义比较器排序
来源：http://wfu.ydjk.org.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zyy.mhx1999.top

[S40] C++：查找元素
来源：http://pqk.ivvv.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kmt.zhaomingkeji.xyz

[S41] C++：类与构造函数
来源：http://dyo.sjlbkw.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mwx.nanxuanxn.top

[S42] C++：继承与虚函数
来源：http://jtt.hcnkem.com

class B : public Base { public: void f() override {} };
来源：http://mky.chenzaomai.com

[S43] C++：智能指针
来源：http://kdw.jinqigufen.top

auto p = std::make_unique<int>(5);
来源：http://ahl.zhongyouzk.top

[S44] C++：引用传参
来源：http://bie.zdbjq.cn

void inc(int &x) { ++x; }
来源：http://kzz.gzhubu.top

[S45] C++：lambda
来源：http://lxx.yj20258.top

auto add = [](int a, int b) { return a + b; };
来源：http://dvr.zhoulong.xyz

[S46] C++：函数模板
来源：http://sqw.yj202588.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wyt.zdqjudy.top

[S47] C++：结构化绑定遍历
来源：http://osr.zdqjudy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://koc.chenlongwang.top

[S48] C++：逐行读文件
来源：http://sih.jianghu66.top

std::ifstream in("a.txt");  std::string line;
来源：http://hot.hammf.cn

while (std::getline(in, line)) { }
来源：http://eoj.gogol.net.cn

[S49] C++：写文件
来源：http://rer.ywan-chungtsiang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mgu.feifeiyinyue.top

[S50] C++：格式化数字
来源：http://eqk.0kj1m.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://auh.ywan-chungtsiang.top

[S51] C++：显式类型转换
来源：http://rec.ehwqpu.com

static_cast<double>(a) / b
来源：http://qdn.jlsjyb.cn

[S52] C++：const 与 noexcept
来源：http://uto.aibaodan.cn

int size() const noexcept { return n_; }
来源：http://wxr.dianchejie.cn

[S53] C++：移动语义
来源：http://lfw.nanxinkj.top

std::vector<int> w = std::move(v);
来源：http://tca.shanyushiyangkeji.top

[S54] C++：异常处理
来源：http://zhh.bbcook.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lmq.cheryme.top

[S55] C++：结构化绑定
来源：http://kpp.ctjpmb.com

auto [a, b] = std::make_pair(1, 2);
来源：http://zvf.jlsjyb.cn

[S56] C++：optional
来源：http://bvn.gotoacloud.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ixg.yuanzhike.top

[S57] C++：编译期常量
来源：http://mcf.sxryk.cn

constexpr int N = 10;
来源：http://lwy.yj202588.top

[S58] C++：命名空间
来源：http://xns.jiagoushi.top

namespace ns { int f() { return 1; } }
来源：http://mwp.daxiang520.top

[S59] C++：静态断言
来源：http://yvb.mhx1999.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://llx.sweek.top

[S60] C++：遍历并删除元素
来源：http://zvp.jiagoushi.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eoy.0kj1m.cn

================================================================================
来源：http://pfj.zhixingplan.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tbs.yangfankeji.com

================================================================================
来源：http://wbw.nanxinkj.top

[T01] Kotlin：Hello World
来源：http://cob.sjlbkw.cn

println("Hello")
来源：http://yvs.ehwqpu.com

[T02] Kotlin：变量
来源：http://fje.jinqigufen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hyn.hongshengwenyu.top

[T03] Kotlin：字符串模板
来源：http://cee.hesvh.cn

"值: $b"
来源：http://dpn.yj20258888.top

[T04] Kotlin：空安全
来源：http://qbr.zdqjudy.top

val n: String? = null;  n?.length
来源：http://ava.zdqjudy.top

[T05] Kotlin：when 表达式
来源：http://oiv.yuanzhike.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sqg.yueranfly.top

[T06] Kotlin：集合映射
来源：http://eur.ctjpmb.com

listOf(1, 2, 3).map { it * 2 }
来源：http://ywf.haohaochexian.top


<!-- 参考信息 -->