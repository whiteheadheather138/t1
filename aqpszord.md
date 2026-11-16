代发 wailian999

name="${1:-default}"
来源：http://yfz.zhengqikj.top

[R06] 判断命令是否存在
来源：http://kli.zhongyouzk.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nkl.tarul.cn

[R07] if 判断文件
来源：http://fqd.ywan-chungtsiang.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://okn.chenzaomai.com

[R08] 数值比较
来源：http://ghi.wangshuangyany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mku.gaohongyu789.top

[R09] 字符串比较
来源：http://qxk.ctjpmb.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yrt.zdqjudy.top

[R10] 正则匹配
来源：http://ypj.316326.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://phu.pycfn.com

[R11] case 多分支
来源：http://txo.jinqigfzy.top

case "$1" in
来源：http://vvv.jlsjyb.cn

start) echo "启动" ;;
来源：http://hgv.aizwys.cn

stop)  echo "停止" ;;
来源：http://zzz.gotoacloud.top

*)     echo "未知命令" ;;
来源：http://uru.jinyuanbaomall.cn

esac
来源：http://vuv.ctjpmb.com

[R12] for 遍历文件
来源：http://oqc.vehdjk.com

for f in *.txt; do echo "$f"; done
来源：http://zvr.nanxinkj.top

[R13] for 计数循环
来源：http://yop.gogol.net.cn

for i in {1..10}; do echo "$i"; done
来源：http://mpd.shangyingyoupin.top

[R14] C 风格 for
来源：http://ypj.jinqigufen.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rem.mhx1999.top

[R15] while 逐行读文件
来源：http://zwa.feifeiyinyue.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://khk.feifeiyinyue.top

[R16] until 等待条件
来源：http://oxp.hfpthk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://czq.jqgfzy.top

[R17] 数组定义与取值
来源：http://cpk.jqgfzy.top

arr=(a b c); echo "${arr[0]}"
来源：http://fcl.hnqzz.top

[R18] 遍历数组
来源：http://mal.jianghu66.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://asy.chenlongwang.top

[R19] 数组长度
来源：http://xgj.jinghuilouyu.cn

echo "${#arr[@]}"
来源：http://eco.cucudq.cn

[R20] 关联数组（字典）
来源：http://ziz.0kj1m.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mmm.316326.xyz

[R21] 字符串长度
来源：http://vyx.sxryk.cn

echo "${#s}"
来源：http://xwh.jqgfzy.top

[R22] 截取子串
来源：http://jsw.snrcjt.cn

echo "${s:0:5}"
来源：http://vbn.yj20258888.top

[R23] 字符串替换
来源：http://aeh.zdbjq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://stc.ctjpmb.com

[R24] 大小写转换
来源：http://eoy.sjlbkw.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jis.sufxvd.cn

[R25] 去后缀 / 去前缀
来源：http://sac.zhongyouzk.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zjh.dianchejie.cn

[R26] 命令替换
来源：http://xof.aibaodan.cn

now=$(date +%F); echo "$now"
来源：http://kzb.yj20258888.top

[R27] 算术展开
来源：http://rey.cdnleiting.top

echo $((1 + 2 * 3))
来源：http://ftj.fktsv.cn

[R28] 浮点运算
来源：http://fqb.daxiang520.top

echo "scale=2; 10/3" | bc
来源：http://ymi.yanxiufei.cn

[R29] 定义函数
来源：http://kqm.jinqigufen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lmg.jinyuanbaomall.cn

[R30] 函数返回状态码
来源：http://pan.yj202588.top

f() { return 0; }; f || echo "失败了"
来源：http://isg.cdnleiting.top

[R31] 局部变量
来源：http://nfy.hcnkem.com

f() { local x=1; echo "$x"; }
来源：http://vyn.yongpay.top

[R32] 参数个数校验
来源：http://jcf.yongpay.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mme.chenlongwang.top

[R33] 捕获错误并提示行号
来源：http://jwn.yj20258.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xmo.hysaishi.cn

[R34] 退出时清理
来源：http://asw.hfpthk.cn

trap 'rm -f "$tmp"' EXIT
来源：http://klw.zhongyouzk.top

[R35] 后台执行并等待
来源：http://scy.ppjwa.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tkc.ydzc1.top

[R36] 并发执行多个任务
来源：http://vzm.0kj1m.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jvh.hywenlv.cn

[R37] 把输出赋给变量
来源：http://iwk.yj20258888.top

files=$(ls -1)
来源：http://umi.andypj.xyz

[R38] 管道串联
来源：http://ufp.ehwqpu.com

cat a.txt | grep -i error | wc -l
来源：http://ras.jqgfzy.top

[R39] 重定向标准输出与错误
来源：http://lav.tian-w.cn

cmd > out.log 2>&1
来源：http://bzt.ydzc1.top

[R40] 追加写日志
来源：http://gcu.jyoumei.cn

echo "log" >> out.log
来源：http://zaf.zdbjq.cn

[R41] 丢弃输出
来源：http://yjk.sufxvd.cn

cmd >/dev/null 2>&1
来源：http://jbq.daria6918.cn

[R42] 输入重定向
来源：http://hkq.yj20258888.top

wc -l < a.txt
来源：http://rdm.vqdsnc.cn

[R43] 按名字查找文件
来源：http://sml.hongshengwenyu.top

find . -name "*.log" -type f
来源：http://jnl.guannengcc.top

[R44] 按修改时间查找
来源：http://gic.sufxvd.cn

find . -mtime -7 -type f
来源：http://rjh.guowangkeji.top

[R45] 批量删除
来源：http://brt.sysykeji.top

find . -name "*.tmp" -delete
来源：http://jmk.kuanghao11.cn

[R46] 递归替换文件内容
来源：http://mrl.jqgufenzy.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fni.redwolf501.top

[R47] sed 单行替换
来源：http://seg.bbcook.cn

sed -i 's/foo/bar/g' a.txt
来源：http://tzb.cashguo.top

[R48] awk 取指定列
来源：http://igb.fengsongda.top

awk '{print $1, $3}' a.txt
来源：http://ouf.jiagoushi.top

[R49] awk 带条件
来源：http://pqv.xingfuxueyuan.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://uir.shanyushiyangtech.top

[R50] awk 求和
来源：http://vjs.zhongyouzk.top

awk '{s += $2} END {print s}' a.txt
来源：http://wze.daxiang520.top

[R51] 排序去重取前几
来源：http://xsd.cdnleiting.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jio.epnwcf.com

[R52] 统计行数
来源：http://hxe.sxryk.cn

wc -l a.txt
来源：http://gja.ivvv.top

[R53] 查看文件头与实时尾
来源：http://ehc.sweek.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://swb.sweek.top

[R54] 比较两个文件
来源：http://zeh.yj20258.top

diff a.txt b.txt
来源：http://mbh.yongpay.top

[R55] 压缩与解压
来源：http://izs.gotoacloud.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bgp.316326.xyz

[R56] 远程拷贝
来源：http://sqg.ehwqpu.com

scp file user@host:/path/
来源：http://npp.zhixingplan.top

[R57] 远程执行命令
来源：http://xzr.ywan-chungtsiang.top

ssh user@host 'uptime'
来源：http://yeh.gaohongyu789.top

[R58] 下载文件
来源：http://inf.ctjpmb.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ick.yuanzhike.top

[R59] 发 POST JSON
来源：http://tga.shzxlz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zfz.zhoulong.xyz

[R60] 只看 HTTP 状态码
来源：http://kig.chenlongwang.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://okc.ctjpmb.com

[R61] 磁盘占用
来源：http://uoy.chenzaomai.com

df -h;  du -sh *
来源：http://zdc.9152youxi.cn

[R62] 找最占空间的文件
来源：http://fwf.hammf.cn

du -ah . | sort -rh | head -10
来源：http://hds.shuidangran.top

[R63] 内存与进程
来源：http://hpy.yuxming.cn

free -h;  ps aux | grep nginx
来源：http://gvd.guowangkeji.top

[R64] 结束进程
来源：http://xxe.wangdashe.top

kill -9 $(pgrep -f app.py)
来源：http://ugu.iojbl.cn

[R65] 查看端口占用
来源：http://lvh.ydjk.org.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cgo.ywan-chungtsiang.top

[R66] 定时任务
来源：http://qld.hongshengwenyu.top

crontab -e;  crontab -l
来源：http://het.fehbvm.com

[R67] 生成随机十六进制串
来源：http://anf.ydjk.org.cn

openssl rand -hex 16
来源：http://zan.shanyushiyangkeji.top

[R68] 计算文件校验值
来源：http://wuy.yangfankeji.com

sha256sum a.txt;  md5sum a.txt
来源：http://fis.sjlbkw.cn

[R69] 生成随机密码
来源：http://biv.daria6918.cn

head -c 16 /dev/urandom | base64
来源：http://qbs.hysaishi.cn

[R70] 时间戳与互转
来源：http://tcn.tian-w.cn

date +%s;  date -d @1700000000
来源：http://gny.shangyingyoupin.top

[R71] 日期格式化
来源：http://ujz.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://jru.fanxiaobao.xyz

[R72] 等待端口就绪
来源：http://kcp.jinyuanbaomall.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wgn.zdqjudy.top

[R73] 分割大日志
来源：http://sgl.yj20258888.top

split -l 1000 big.log part_
来源：http://ges.chenzaomai.com

[R74] 批量重命名
来源：http://tjo.hnxiangtu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jnu.pycfn.com

[R75] 导出环境变量
来源：http://dkd.yvedp.cn

export PATH="$HOME/bin:$PATH"
来源：http://hhy.hnqzz.top

[R76] 使用临时文件
来源：http://qho.jinqigfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://pqg.hysaishi.cn

[R77] 读取用户输入
来源：http://cob.aizwys.cn

read -rp "请输入: " ans
来源：http://lmg.hywenlv.cn

[R78] 交互式菜单
来源：http://zgm.zhongyouzk.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qmw.hongshengwenyu.top

[R79] 解析命令行选项
来源：http://zme.tanke756.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://atn.nanxinkj.top

[R80] 查看脚本执行耗时
来源：http://zbj.316326.xyz

time ./run.sh
来源：http://wtg.aibaodan.cn

================================================================================
来源：http://gwr.jinghuilouyu.cn

S. C / C++ 专题
来源：http://tef.zhijiandao.cn

================================================================================
来源：http://jsc.jlsjyb.cn

[S01] C：Hello World
来源：http://sua.pycfn.com

#include <stdio.h>
来源：http://kwh.hcnkem.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://ikc.ydjk.org.cn

[S02] C：变量与格式化输出
来源：http://kam.shanyushiyangtech.top

int a = 10; printf("%d\n", a);
来源：http://ybg.ydzc1.top

[S03] C：读入整数
来源：http://gja.pycfn.com

int x; scanf("%d", &x);
来源：http://ope.chenjidiqi.icu

[S04] C：字符串复制
来源：http://wkj.yvedp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lev.yonumen.top

[S05] C：字符串长度
来源：http://nle.ppjwa.cn

strlen(s)
来源：http://vcs.guowangkeji.top

[S06] C：字符串比较
来源：http://mhn.316326.xyz

strcmp(a, b) == 0
来源：http://dqy.fanxiaobao.xyz

[S07] C：数组遍历求和
来源：http://fhe.shanyushiyangtech.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pbf.yj202588.top

[S08] C：动态内存分配与释放
来源：http://mtf.cucudq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vpj.tian-w.cn

[S09] C：结构体定义与初始化
来源：http://zpa.yueranfly.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hwc.epnwcf.com

[S10] C：指针与解引用
来源：http://umu.zhoulong.xyz

int *p = &a;  *p = 5;
来源：http://ycb.hysaishi.cn

[S11] C：逐行读文件
来源：http://uss.jqgufenzy.top

FILE *f = fopen("a.txt", "r");
来源：http://nra.chenzaomai.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://tjy.shzxlz.cn

fclose(f);
来源：http://ksq.shanyushiyangkeji.top

[S12] C：写文件
来源：http://guk.havefunace.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hee.snrcjt.cn

[S13] C：宏定义
来源：http://nms.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yay.yuanzhike.top

[S14] C：枚举
来源：http://sir.hcnkem.com

enum Color { RED, GREEN, BLUE };
来源：http://urv.chenjidiqi.icu

[S15] C：类型转换
来源：http://ilu.cheryme.top

(double) a / b
来源：http://djw.chenlongwang.top

[S16] C：位操作置位
来源：http://ekb.shzxlz.cn

x |= (1 << 3);
来源：http://fqs.dianchejie.cn

[S17] C：安全拼接字符串
来源：http://kel.cashguo.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jwm.hnqzz.top

[S18] C：命令行参数
来源：http://cst.ehwqpu.com

int main(int argc, char **argv)
来源：http://wva.zhoulong.xyz

[S19] C：快速排序
来源：http://kzk.hnqzz.top

qsort(a, n, sizeof(int), cmp);
来源：http://vyf.chenjidiqi.icu

[S20] C：二分查找
来源：http://snm.pengpengdd.cyou

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wpz.fktsv.cn

[S21] C：字符类别判断
来源：http://smw.andypj.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://iii.chenzaomai.com

[S22] C：字符串转数字
来源：http://ija.quarkkingdee.top

atoi("42");  strtod("3.14", NULL);
来源：http://gbw.cdnleiting.top

[S23] C：随机数
来源：http://htx.shuidangran.top

srand(time(NULL));  int r = rand() % 100;
来源：http://eqm.52xcode.cn

[S24] C：获取本地时间
来源：http://kce.meibo888.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://csq.hnxiangtu.top

[S25] C：内存拷贝
来源：http://ggz.aizwys.cn

memcpy(dst, src, n);
来源：http://cdq.cucudq.cn

[S26] C：内存清零
来源：http://ojf.pycfn.com

memset(a, 0, sizeof a);
来源：http://rve.jinghuilouyu.cn

[S27] C：定义常量
来源：http://pfm.zhijiandao.cn

const double PI = 3.14159;
来源：http://biq.jlsjyb.cn

[S28] C：静态变量
来源：http://sse.bbcook.cn

static int counter = 0;
来源：http://fjh.sweek.top

[S29] C：变参函数
来源：http://zlp.zhaomingkeji.xyz

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ajm.redwolf501.top

[S30] C：头文件保护
来源：http://jcc.ywan-chungtsiang.top

#ifndef X_H
来源：http://lxo.zhongyouzk.top

#define X_H
来源：http://fip.xylfe.cn

#endif
来源：http://lan.tanke756.top

[S31] C++：Hello World
来源：http://jkg.zhoulong.xyz

#include <iostream>
来源：http://nhw.zhengqikj.top

int main() { std::cout << "Hello\n"; }
来源：http://kra.gogol.net.cn

[S32] C++：字符串
来源：http://mvq.xylfe.cn

std::string s = "hi";  s += "!";
来源：http://npd.sufxvd.cn

[S33] C++：vector 增删
来源：http://nhp.xinyue.icu

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tbd.zhijiandao.cn

[S34] C++：遍历 vector
来源：http://ieh.c1oappe.top

for (auto &x : v) { std::cout << x; }
来源：http://slr.yueranfly.top

[S35] C++：map
来源：http://heb.zhaomingkeji.xyz

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nfu.havefunace.top

[S36] C++：unordered_map
来源：http://enj.yfazqb.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ayb.jyoumei.cn

[S37] C++：set
来源：http://amq.yj20258.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wns.yvedp.cn

[S38] C++：排序
来源：http://ecs.ydjk.org.cn

std::sort(v.begin(), v.end());
来源：http://muf.fktsv.cn

[S39] C++：自定义比较器排序
来源：http://uip.zhiwuduotai.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jqg.tianlin.xyz

[S40] C++：查找元素
来源：http://vdw.xuetiantiany.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ela.wangdashe.top

[S41] C++：类与构造函数
来源：http://kij.zycfv.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://azo.yuxming.cn

[S42] C++：继承与虚函数
来源：http://oiy.shanyushiyangkeji.top

class B : public Base { public: void f() override {} };
来源：http://ivx.feifeiyinyue.top

[S43] C++：智能指针
来源：http://fzp.tarul.cn

auto p = std::make_unique<int>(5);
来源：http://vlq.dianchejie.cn

[S44] C++：引用传参
来源：http://gkm.316326.xyz

void inc(int &x) { ++x; }
来源：http://bba.chenjidiqi.icu

[S45] C++：lambda
来源：http://ngl.sysykeji.top

auto add = [](int a, int b) { return a + b; };
来源：http://kes.zycfv.cn

[S46] C++：函数模板
来源：http://ozg.tarul.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mrj.havefunace.top

[S47] C++：结构化绑定遍历
来源：http://afd.yueranfly.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jsq.zdqjudy.top

[S48] C++：逐行读文件
来源：http://vom.ivvv.top

std::ifstream in("a.txt");  std::string line;
来源：http://vqs.wangdashe.top

while (std::getline(in, line)) { }
来源：http://xbn.9152youxi.cn

[S49] C++：写文件
来源：http://hnb.chenlongwang.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ivq.yongpay.top

[S50] C++：格式化数字
来源：http://dpt.redwolf501.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mes.ehwqpu.com

[S51] C++：显式类型转换
来源：http://wsh.havefunace.top

static_cast<double>(a) / b
来源：http://hoe.sweek.top

[S52] C++：const 与 noexcept
来源：http://qvw.andypj.xyz

int size() const noexcept { return n_; }
来源：http://dqu.yj20258888.top

[S53] C++：移动语义
来源：http://ytd.daxiang520.top

std::vector<int> w = std::move(v);
来源：http://ajh.kuanghao11.cn

[S54] C++：异常处理
来源：http://bxi.jqgfzy.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bkb.yfazqb.com

[S55] C++：结构化绑定
来源：http://pfl.aibaodan.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://thk.zhengqikj.top

[S56] C++：optional
来源：http://jhe.gogol.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ydo.hesvh.cn

[S57] C++：编译期常量
来源：http://pbs.ydjk.org.cn

constexpr int N = 10;
来源：http://hjz.wangshuangyany.cn

[S58] C++：命名空间
来源：http://rtv.chenjidiqi.icu

namespace ns { int f() { return 1; } }
来源：http://tjb.yfazqb.com

[S59] C++：静态断言
来源：http://zxt.daxiang520.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dmo.nwbrower.top

[S60] C++：遍历并删除元素
来源：http://vpx.jianghu66.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fyw.redwolf501.top

================================================================================
来源：http://hpc.yvedp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://isv.xinyue.icu

================================================================================
来源：http://poc.haohaochexian.top

[T01] Kotlin：Hello World
来源：http://rdu.guowangkeji.top

println("Hello")
来源：http://rmm.shangyingyoupin.top

[T02] Kotlin：变量
来源：http://nrc.pengpengdd.cyou

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mtk.andypj.xyz

[T03] Kotlin：字符串模板
来源：http://dlr.iojbl.cn

"值: $b"
来源：http://nri.bbcook.cn

[T04] Kotlin：空安全
来源：http://eng.hongshengwenyu.top

val n: String? = null;  n?.length
来源：http://zis.hywenlv.cn

[T05] Kotlin：when 表达式
来源：http://xwz.jyoumei.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hru.cheryme.top

[T06] Kotlin：集合映射
来源：http://vyb.dashuyun.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gpc.hywenlv.cn


<!-- 参考信息 -->