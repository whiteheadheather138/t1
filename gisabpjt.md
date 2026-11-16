代发 wailian999

set -euo pipefail
来源：http://lxo.gotoacloud.top

[R02] 变量赋值与使用
来源：http://pof.guowangkeji.top

name="Tom"; echo "$name"
来源：http://pnp.chenjidiqi.icu

[R03] 只读变量
来源：http://yqb.zhaomingkeji.xyz

readonly PI=3.14
来源：http://ohz.wangshuangyany.cn

[R04] 位置参数
来源：http://trk.hnxiangtu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tpo.fktsv.cn

[R05] 参数默认值
来源：http://jtd.snrcjt.cn

name="${1:-default}"
来源：http://ngj.epnwcf.com

[R06] 判断命令是否存在
来源：http://crp.daria6918.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ggw.zhijiandao.cn

[R07] if 判断文件
来源：http://mul.dashuyun.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hhu.fengsongda.top

[R08] 数值比较
来源：http://odg.ppjwa.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://tji.shuidangran.top

[R09] 字符串比较
来源：http://qlh.pycfn.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://eer.gaohongyu789.top

[R10] 正则匹配
来源：http://fxs.fengsongda.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fcx.9152youxi.cn

[R11] case 多分支
来源：http://pac.xinyue.icu

case "$1" in
来源：http://apw.tarul.cn

start) echo "启动" ;;
来源：http://avv.redwolf501.top

stop)  echo "停止" ;;
来源：http://ygz.xylfe.cn

*)     echo "未知命令" ;;
来源：http://uhf.ehwqpu.com

esac
来源：http://qah.andypj.xyz

[R12] for 遍历文件
来源：http://cdv.jiagoushi.top

for f in *.txt; do echo "$f"; done
来源：http://twi.ppjwa.cn

[R13] for 计数循环
来源：http://crw.shanyushiyangtech.top

for i in {1..10}; do echo "$i"; done
来源：http://qxq.jinyuanbaomall.cn

[R14] C 风格 for
来源：http://igl.snrcjt.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xcq.havefunace.top

[R15] while 逐行读文件
来源：http://xxc.jiagoushi.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qtg.xylfe.cn

[R16] until 等待条件
来源：http://asw.gzhubu.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wbv.ehwqpu.com

[R17] 数组定义与取值
来源：http://rte.epnwcf.com

arr=(a b c); echo "${arr[0]}"
来源：http://gwn.wangdashe.top

[R18] 遍历数组
来源：http://lyv.sxryk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://syz.yj202588.top

[R19] 数组长度
来源：http://gvc.fanxiaobao.xyz

echo "${#arr[@]}"
来源：http://jdk.jqgfzy.top

[R20] 关联数组（字典）
来源：http://isq.cheryme.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fza.ehwqpu.com

[R21] 字符串长度
来源：http://itx.zhijiandao.cn

echo "${#s}"
来源：http://cmv.havefunace.top

[R22] 截取子串
来源：http://rhv.xuetiantiany.cn

echo "${s:0:5}"
来源：http://oap.gzhubu.top

[R23] 字符串替换
来源：http://bef.jinyuanbaomall.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://apw.havefunace.top

[R24] 大小写转换
来源：http://hni.wangdashe.top

echo "${s^^}"; echo "${s,,}"
来源：http://rki.shuidangran.top

[R25] 去后缀 / 去前缀
来源：http://nsi.andypj.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://oqg.andypj.xyz

[R26] 命令替换
来源：http://hiu.nanxinkj.top

now=$(date +%F); echo "$now"
来源：http://qkr.tarul.cn

[R27] 算术展开
来源：http://doi.sxryk.cn

echo $((1 + 2 * 3))
来源：http://jpw.yj20258.top

[R28] 浮点运算
来源：http://fij.nwbrower.top

echo "scale=2; 10/3" | bc
来源：http://yqw.yj20258888.top

[R29] 定义函数
来源：http://ozv.fktsv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://fmx.iojbl.cn

[R30] 函数返回状态码
来源：http://xxi.xuanzx.com

f() { return 0; }; f || echo "失败了"
来源：http://flo.gotoacloud.top

[R31] 局部变量
来源：http://lub.jianghu66.top

f() { local x=1; echo "$x"; }
来源：http://dhb.daxiang520.top

[R32] 参数个数校验
来源：http://gfe.xuetiantiany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://qyu.daxiang520.top

[R33] 捕获错误并提示行号
来源：http://isa.pycfn.com

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jvq.ydzc1.top

[R34] 退出时清理
来源：http://cat.kuanghao11.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dop.ydzc1.top

[R35] 后台执行并等待
来源：http://nec.hywenlv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ddt.redwolf501.top

[R36] 并发执行多个任务
来源：http://cpn.cdnleiting.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cci.zhixingplan.top

[R37] 把输出赋给变量
来源：http://gdf.cheryme.top

files=$(ls -1)
来源：http://qrg.yongpay.top

[R38] 管道串联
来源：http://kag.uphjek.com

cat a.txt | grep -i error | wc -l
来源：http://noh.cashguo.top

[R39] 重定向标准输出与错误
来源：http://rsk.yongpay.top

cmd > out.log 2>&1
来源：http://znk.meibo888.top

[R40] 追加写日志
来源：http://bmr.snrcjt.cn

echo "log" >> out.log
来源：http://rmu.andypj.xyz

[R41] 丢弃输出
来源：http://lkb.yonumen.top

cmd >/dev/null 2>&1
来源：http://ahn.yueranfly.top

[R42] 输入重定向
来源：http://tgs.smart0.xyz

wc -l < a.txt
来源：http://ulw.chenlongwang.top

[R43] 按名字查找文件
来源：http://zwr.redwolf501.top

find . -name "*.log" -type f
来源：http://hsw.xylfe.cn

[R44] 按修改时间查找
来源：http://nbe.shanyushiyangkeji.top

find . -mtime -7 -type f
来源：http://smp.aizwys.cn

[R45] 批量删除
来源：http://xun.zdqjudy.top

find . -name "*.tmp" -delete
来源：http://sbt.shanyushiyangtech.top

[R46] 递归替换文件内容
来源：http://bwh.jinqigfzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sly.zhengqikj.top

[R47] sed 单行替换
来源：http://ztn.quarkkingdee.top

sed -i 's/foo/bar/g' a.txt
来源：http://zdy.9152youxi.cn

[R48] awk 取指定列
来源：http://ovr.316326.xyz

awk '{print $1, $3}' a.txt
来源：http://jkc.jianghu66.top

[R49] awk 带条件
来源：http://ubr.jqgufenzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wpd.shuidangran.top

[R50] awk 求和
来源：http://ryk.52xcode.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mih.hysaishi.cn

[R51] 排序去重取前几
来源：http://dle.zhoulong.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://mat.jiagoushi.top

[R52] 统计行数
来源：http://bid.jqgufenzy.top

wc -l a.txt
来源：http://aio.bjfxy.top

[R53] 查看文件头与实时尾
来源：http://dgn.hysaishi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gey.jqgfzy.top

[R54] 比较两个文件
来源：http://zod.gaohongyu789.top

diff a.txt b.txt
来源：http://rog.hnxiangtu.top

[R55] 压缩与解压
来源：http://tef.hywenlv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nix.xziqi.cn

[R56] 远程拷贝
来源：http://mjt.daria6918.cn

scp file user@host:/path/
来源：http://owy.tanke756.top

[R57] 远程执行命令
来源：http://bsk.hnxiangtu.top

ssh user@host 'uptime'
来源：http://hre.shanyushiyangtech.top

[R58] 下载文件
来源：http://vwh.sufxvd.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dzi.mhx1999.top

[R59] 发 POST JSON
来源：http://fkm.yueranfly.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vhm.gotoacloud.top

[R60] 只看 HTTP 状态码
来源：http://mse.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ebz.yangfankeji.com

[R61] 磁盘占用
来源：http://cci.iojbl.cn

df -h;  du -sh *
来源：http://nap.fengsongda.top

[R62] 找最占空间的文件
来源：http://xzh.yonumen.top

du -ah . | sort -rh | head -10
来源：http://wvk.hfpthk.cn

[R63] 内存与进程
来源：http://nls.meibo888.top

free -h;  ps aux | grep nginx
来源：http://wyg.zhengqikj.top

[R64] 结束进程
来源：http://vav.yuanzhike.top

kill -9 $(pgrep -f app.py)
来源：http://jaz.birdmap.top

[R65] 查看端口占用
来源：http://bvv.zhijiandao.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wwg.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://qah.bbcook.cn

crontab -e;  crontab -l
来源：http://ewk.bbcook.cn

[R67] 生成随机十六进制串
来源：http://ujy.svipenyu.cn

openssl rand -hex 16
来源：http://yrh.jinqigfzy.top

[R68] 计算文件校验值
来源：http://dpc.ehwqpu.com

sha256sum a.txt;  md5sum a.txt
来源：http://ery.bjfxy.top

[R69] 生成随机密码
来源：http://eut.zhoulong.xyz

head -c 16 /dev/urandom | base64
来源：http://anb.zdbjq.cn

[R70] 时间戳与互转
来源：http://vcf.jlsjyb.cn

date +%s;  date -d @1700000000
来源：http://zol.xingfuxueyuan.xyz

[R71] 日期格式化
来源：http://gia.tarul.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kwk.jinghuilouyu.cn

[R72] 等待端口就绪
来源：http://jki.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://ktx.sysykeji.top

[R73] 分割大日志
来源：http://eey.vehdjk.com

split -l 1000 big.log part_
来源：http://mkr.9152youxi.cn

[R74] 批量重命名
来源：http://fir.feifeiyinyue.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kqk.jianghu66.top

[R75] 导出环境变量
来源：http://quw.svipenyu.cn

export PATH="$HOME/bin:$PATH"
来源：http://bzq.ppjwa.cn

[R76] 使用临时文件
来源：http://fzj.zhongyouzk.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://cuj.yueranfly.top

[R77] 读取用户输入
来源：http://ohh.zhijiandao.cn

read -rp "请输入: " ans
来源：http://xpv.jiagoushi.top

[R78] 交互式菜单
来源：http://yvt.jlsjyb.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uhh.jinghuilouyu.cn

[R79] 解析命令行选项
来源：http://lwq.jinqigufen.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dtg.52xcode.cn

[R80] 查看脚本执行耗时
来源：http://fvb.pycfn.com

time ./run.sh
来源：http://qav.wangshuangyany.cn

================================================================================
来源：http://lfv.cucudq.cn

S. C / C++ 专题
来源：http://wff.yueranfly.top

================================================================================
来源：http://ffu.jinqigufen.top

[S01] C：Hello World
来源：http://ons.cashguo.top

#include <stdio.h>
来源：http://zsh.yueranfly.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://xbx.epnwcf.com

[S02] C：变量与格式化输出
来源：http://tzo.chenjidiqi.icu

int a = 10; printf("%d\n", a);
来源：http://tvm.cdnleiting.top

[S03] C：读入整数
来源：http://aeu.xziqi.cn

int x; scanf("%d", &x);
来源：http://iht.ivvv.top

[S04] C：字符串复制
来源：http://sht.yueranfly.top

char dst[32]; strcpy(dst, "hi");
来源：http://ubs.zhoulong.xyz

[S05] C：字符串长度
来源：http://lvt.fanxiaobao.xyz

strlen(s)
来源：http://yxx.9152youxi.cn

[S06] C：字符串比较
来源：http://lml.zhengqikj.top

strcmp(a, b) == 0
来源：http://mfp.shuidangran.top

[S07] C：数组遍历求和
来源：http://sqr.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hbx.fzhhl.top

[S08] C：动态内存分配与释放
来源：http://css.yj202588.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wjs.wangshuangyany.cn

[S09] C：结构体定义与初始化
来源：http://weg.fzhhl.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wqm.xuanzx.com

[S10] C：指针与解引用
来源：http://kbd.hysaishi.cn

int *p = &a;  *p = 5;
来源：http://vah.jqgufenzy.top

[S11] C：逐行读文件
来源：http://yfn.smart0.xyz

FILE *f = fopen("a.txt", "r");
来源：http://fpl.iojbl.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pmw.xingfuxueyuan.xyz

fclose(f);
来源：http://buo.sysykeji.top

[S12] C：写文件
来源：http://sic.hongshengwenyu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bsn.ywan-chungtsiang.top

[S13] C：宏定义
来源：http://ueb.nwbrower.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yfc.sufxvd.cn

[S14] C：枚举
来源：http://rdp.fehbvm.com

enum Color { RED, GREEN, BLUE };
来源：http://dwv.jianghu66.top

[S15] C：类型转换
来源：http://pzs.yj20258.top

(double) a / b
来源：http://umy.shanyushiyangtech.top

[S16] C：位操作置位
来源：http://dgn.pycfn.com

x |= (1 << 3);
来源：http://vka.cashguo.top

[S17] C：安全拼接字符串
来源：http://mce.redwolf501.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dgz.feifeiyinyue.top

[S18] C：命令行参数
来源：http://vjb.meibo888.top

int main(int argc, char **argv)
来源：http://syd.tanke756.top

[S19] C：快速排序
来源：http://fri.xuanzx.com

qsort(a, n, sizeof(int), cmp);
来源：http://vwl.ctjpmb.com

[S20] C：二分查找
来源：http://qtf.hongshengwenyu.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mmn.fanxiaobao.xyz

[S21] C：字符类别判断
来源：http://kng.yfazqb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zlu.daria6918.cn

[S22] C：字符串转数字
来源：http://oed.bjfxy.top

atoi("42");  strtod("3.14", NULL);
来源：http://khf.jlsjyb.cn

[S23] C：随机数
来源：http://dmq.dashuyun.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://awf.ivvv.top

[S24] C：获取本地时间
来源：http://hck.cqqwz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ehb.jqgufenzy.top

[S25] C：内存拷贝
来源：http://kny.tarul.cn

memcpy(dst, src, n);
来源：http://mps.zycfv.cn

[S26] C：内存清零
来源：http://dpq.xuetiantiany.cn

memset(a, 0, sizeof a);
来源：http://exc.yj202588.top

[S27] C：定义常量
来源：http://jdr.fktsv.cn

const double PI = 3.14159;
来源：http://idl.xingfuxueyuan.xyz

[S28] C：静态变量
来源：http://lmy.xinyue.icu

static int counter = 0;
来源：http://rwu.nanxuanxn.top

[S29] C：变参函数
来源：http://tfq.hammf.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gzo.xuanzx.com

[S30] C：头文件保护
来源：http://mme.ctjpmb.com

#ifndef X_H
来源：http://ogz.jinqigufen.top

#define X_H
来源：http://owm.gaohongyu789.top

#endif
来源：http://dre.chenzaomai.com

[S31] C++：Hello World
来源：http://asc.andypj.xyz

#include <iostream>
来源：http://qsz.meibo888.top

int main() { std::cout << "Hello\n"; }
来源：http://vnx.tian-w.cn

[S32] C++：字符串
来源：http://ipb.jiagoushi.top

std::string s = "hi";  s += "!";
来源：http://eon.hesvh.cn

[S33] C++：vector 增删
来源：http://hqn.vqdsnc.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://oix.316326.xyz

[S34] C++：遍历 vector
来源：http://zgi.yfazqb.com

for (auto &x : v) { std::cout << x; }
来源：http://kzl.gotoacloud.top

[S35] C++：map
来源：http://bsb.jinyuanbaomall.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://awe.yuxming.cn

[S36] C++：unordered_map
来源：http://gam.havefunace.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://iiu.sufxvd.cn

[S37] C++：set
来源：http://qnd.cdnleiting.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ofz.wangshuangyany.cn

[S38] C++：排序
来源：http://ktb.hnqzz.top

std::sort(v.begin(), v.end());
来源：http://nct.shangyingyoupin.top

[S39] C++：自定义比较器排序
来源：http://emb.hnxiangtu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ykw.zycfv.cn

[S40] C++：查找元素
来源：http://iph.jlsjyb.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ita.daxiang520.top

[S41] C++：类与构造函数
来源：http://gzb.fktsv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oxp.fzhhl.top

[S42] C++：继承与虚函数
来源：http://gkh.gotoacloud.top

class B : public Base { public: void f() override {} };
来源：http://xwf.feifeiyinyue.top

[S43] C++：智能指针
来源：http://ckq.hammf.cn

auto p = std::make_unique<int>(5);
来源：http://vrt.andypj.xyz

[S44] C++：引用传参
来源：http://txw.0kj1m.cn

void inc(int &x) { ++x; }
来源：http://tip.hesvh.cn

[S45] C++：lambda
来源：http://xic.chenjidiqi.icu

auto add = [](int a, int b) { return a + b; };
来源：http://uwg.9152youxi.cn

[S46] C++：函数模板
来源：http://gle.ybcxt.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qng.yj202588.top

[S47] C++：结构化绑定遍历
来源：http://jxd.andypj.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jjq.dashuyun.cn

[S48] C++：逐行读文件
来源：http://tbc.hongshengwenyu.top

std::ifstream in("a.txt");  std::string line;
来源：http://cdh.shanyushiyangkeji.top

while (std::getline(in, line)) { }
来源：http://kni.cqqwz.cn

[S49] C++：写文件
来源：http://ovq.ydjk.org.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fjw.hnxiangtu.top

[S50] C++：格式化数字
来源：http://jma.andypj.xyz

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pgc.zdqjudy.top

[S51] C++：显式类型转换
来源：http://ivj.yj20258.top

static_cast<double>(a) / b
来源：http://ogk.iojbl.cn

[S52] C++：const 与 noexcept
来源：http://jjs.ppjwa.cn

int size() const noexcept { return n_; }
来源：http://ayz.gaohongyu789.top

[S53] C++：移动语义
来源：http://cdx.sweek.top

std::vector<int> w = std::move(v);
来源：http://mjf.zhiwuduotai.top

[S54] C++：异常处理
来源：http://dvs.yongpay.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bcf.bjfxy.top

[S55] C++：结构化绑定
来源：http://gdz.zhoulong.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://fhq.vqdsnc.cn

[S56] C++：optional
来源：http://nvg.chenjidiqi.icu

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yem.yanxiufei.cn

[S57] C++：编译期常量
来源：http://rxa.hesvh.cn

constexpr int N = 10;
来源：http://qme.hcnkem.com

[S58] C++：命名空间
来源：http://dkv.gogol.net.cn

namespace ns { int f() { return 1; } }
来源：http://lng.birdmap.top

[S59] C++：静态断言
来源：http://fjj.bjfxy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ibr.yonumen.top

[S60] C++：遍历并删除元素
来源：http://inu.wangshuangyany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://tyj.jlsjyb.cn

================================================================================
来源：http://adw.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vxg.shzxlz.cn

================================================================================
来源：http://zoy.jinqigfzy.top

[T01] Kotlin：Hello World
来源：http://ped.zhiwuduotai.top

println("Hello")
来源：http://sgb.xingfuxueyuan.xyz

[T02] Kotlin：变量
来源：http://ops.nanxuanxn.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hqz.aizwys.cn


<!-- 参考信息 -->