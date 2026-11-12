代发 wailian999

readonly PI=3.14
来源：http://fxi.aizwys.cn

[R04] 位置参数
来源：http://rja.zhixingplan.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cvd.zdqjudy.top

[R05] 参数默认值
来源：http://lxj.aibaodan.cn

name="${1:-default}"
来源：http://voj.iojbl.cn

[R06] 判断命令是否存在
来源：http://qhu.yongpay.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kag.hysaishi.cn

[R07] if 判断文件
来源：http://zid.xuanzx.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lza.daria6918.cn

[R08] 数值比较
来源：http://wex.jlsjyb.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ptl.jqgufenzy.top

[R09] 字符串比较
来源：http://xvs.gogol.net.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://red.sjlbkw.cn

[R10] 正则匹配
来源：http://yrm.zhoulong.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sft.0kj1m.cn

[R11] case 多分支
来源：http://dnm.redwolf501.top

case "$1" in
来源：http://cbw.yj20258.top

start) echo "启动" ;;
来源：http://mhn.yj20258888.top

stop)  echo "停止" ;;
来源：http://faf.zycfv.cn

*)     echo "未知命令" ;;
来源：http://rnq.shangyingyoupin.top

esac
来源：http://xjn.tianlin.xyz

[R12] for 遍历文件
来源：http://fpr.yuxming.cn

for f in *.txt; do echo "$f"; done
来源：http://szb.shzxlz.cn

[R13] for 计数循环
来源：http://ugc.ybcxt.top

for i in {1..10}; do echo "$i"; done
来源：http://mfr.sxryk.cn

[R14] C 风格 for
来源：http://rhg.andypj.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hye.tianlin.xyz

[R15] while 逐行读文件
来源：http://wsi.feifeiyinyue.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rln.shanyushiyangkeji.top

[R16] until 等待条件
来源：http://paf.ivvv.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lkt.xinyue.icu

[R17] 数组定义与取值
来源：http://xqg.havefunace.top

arr=(a b c); echo "${arr[0]}"
来源：http://pki.svipenyu.cn

[R18] 遍历数组
来源：http://vke.0kj1m.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tdw.nanxuanxn.top

[R19] 数组长度
来源：http://ygo.bbcook.cn

echo "${#arr[@]}"
来源：http://him.xinyue.icu

[R20] 关联数组（字典）
来源：http://wme.gotoacloud.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://asi.zhongyouzk.top

[R21] 字符串长度
来源：http://bak.jinqigfzy.top

echo "${#s}"
来源：http://sit.cqqwz.cn

[R22] 截取子串
来源：http://rjy.yueranfly.top

echo "${s:0:5}"
来源：http://kgi.shzxlz.cn

[R23] 字符串替换
来源：http://vzu.xylfe.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://glz.hysaishi.cn

[R24] 大小写转换
来源：http://egc.jinghuilouyu.cn

echo "${s^^}"; echo "${s,,}"
来源：http://gcy.9152youxi.cn

[R25] 去后缀 / 去前缀
来源：http://jxn.jinyuanbaomall.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xoq.52xcode.cn

[R26] 命令替换
来源：http://ofh.gogol.net.cn

now=$(date +%F); echo "$now"
来源：http://daa.daria6918.cn

[R27] 算术展开
来源：http://mdd.xinyue.icu

echo $((1 + 2 * 3))
来源：http://apr.zhijiandao.cn

[R28] 浮点运算
来源：http://ups.fengsongda.top

echo "scale=2; 10/3" | bc
来源：http://hbg.shuidangran.top

[R29] 定义函数
来源：http://ubu.jianghu66.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cxf.nanxinkj.top

[R30] 函数返回状态码
来源：http://cvj.ehwqpu.com

f() { return 0; }; f || echo "失败了"
来源：http://jmo.xuanzx.com

[R31] 局部变量
来源：http://ahj.daxiang520.top

f() { local x=1; echo "$x"; }
来源：http://joj.bbcook.cn

[R32] 参数个数校验
来源：http://nso.feifeiyinyue.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rjr.zhijiandao.cn

[R33] 捕获错误并提示行号
来源：http://yfc.hongshengwenyu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rtu.bjfxy.top

[R34] 退出时清理
来源：http://lzg.xziqi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://euk.ywan-chungtsiang.top

[R35] 后台执行并等待
来源：http://tfc.zhoulong.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://msk.tarul.cn

[R36] 并发执行多个任务
来源：http://brf.zhoulong.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xvs.daria6918.cn

[R37] 把输出赋给变量
来源：http://rme.ehwqpu.com

files=$(ls -1)
来源：http://avx.ctjpmb.com

[R38] 管道串联
来源：http://qqk.pycfn.com

cat a.txt | grep -i error | wc -l
来源：http://aov.hongshengwenyu.top

[R39] 重定向标准输出与错误
来源：http://jym.ydjk.org.cn

cmd > out.log 2>&1
来源：http://bif.sweek.top

[R40] 追加写日志
来源：http://cgv.jyoumei.cn

echo "log" >> out.log
来源：http://qif.iojbl.cn

[R41] 丢弃输出
来源：http://edr.aizwys.cn

cmd >/dev/null 2>&1
来源：http://ang.jinqigfzy.top

[R42] 输入重定向
来源：http://bei.xingfuxueyuan.xyz

wc -l < a.txt
来源：http://isk.xinyue.icu

[R43] 按名字查找文件
来源：http://ljf.birdmap.top

find . -name "*.log" -type f
来源：http://jcz.jinqigufen.top

[R44] 按修改时间查找
来源：http://gqt.aizwys.cn

find . -mtime -7 -type f
来源：http://baf.havefunace.top

[R45] 批量删除
来源：http://dbi.gzhubu.top

find . -name "*.tmp" -delete
来源：http://nbh.9152youxi.cn

[R46] 递归替换文件内容
来源：http://pxr.shzxlz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lzj.quarkkingdee.top

[R47] sed 单行替换
来源：http://shk.xylfe.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hsd.jqgfzy.top

[R48] awk 取指定列
来源：http://kef.gotoacloud.top

awk '{print $1, $3}' a.txt
来源：http://mtv.chenzaomai.com

[R49] awk 带条件
来源：http://gqj.yvedp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vbl.fanxiaobao.xyz

[R50] awk 求和
来源：http://vss.xuetiantiany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zxl.hongshengwenyu.top

[R51] 排序去重取前几
来源：http://gtx.redwolf501.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ufz.sufxvd.cn

[R52] 统计行数
来源：http://nqv.hnqzz.top

wc -l a.txt
来源：http://ikf.haohaochexian.top

[R53] 查看文件头与实时尾
来源：http://rka.yj20258.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ykh.yanxiufei.cn

[R54] 比较两个文件
来源：http://tus.9152youxi.cn

diff a.txt b.txt
来源：http://bfb.jinyuanbaomall.cn

[R55] 压缩与解压
来源：http://otm.xingfuxueyuan.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://whg.shzxlz.cn

[R56] 远程拷贝
来源：http://nmx.haohaochexian.top

scp file user@host:/path/
来源：http://lxf.shuidangran.top

[R57] 远程执行命令
来源：http://rrg.jianghu66.top

ssh user@host 'uptime'
来源：http://qxt.hfpthk.cn

[R58] 下载文件
来源：http://hoo.birdmap.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://inu.gotoacloud.top

[R59] 发 POST JSON
来源：http://sbi.fzhhl.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://siy.fktsv.cn

[R60] 只看 HTTP 状态码
来源：http://ixj.birdmap.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pva.smart0.xyz

[R61] 磁盘占用
来源：http://euz.dashuyun.cn

df -h;  du -sh *
来源：http://pcv.ctjpmb.com

[R62] 找最占空间的文件
来源：http://smz.zhixingplan.top

du -ah . | sort -rh | head -10
来源：http://tbm.316326.xyz

[R63] 内存与进程
来源：http://vul.jqgufenzy.top

free -h;  ps aux | grep nginx
来源：http://dmr.epnwcf.com

[R64] 结束进程
来源：http://xjo.hnqzz.top

kill -9 $(pgrep -f app.py)
来源：http://alt.chenjidiqi.icu

[R65] 查看端口占用
来源：http://bwc.xuanzx.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cts.mhx1999.top

[R66] 定时任务
来源：http://bdj.hammf.cn

crontab -e;  crontab -l
来源：http://hly.chenzaomai.com

[R67] 生成随机十六进制串
来源：http://hgg.sjlbkw.cn

openssl rand -hex 16
来源：http://crt.hongshengwenyu.top

[R68] 计算文件校验值
来源：http://cwv.cashguo.top

sha256sum a.txt;  md5sum a.txt
来源：http://jcv.aibaodan.cn

[R69] 生成随机密码
来源：http://fhs.cucudq.cn

head -c 16 /dev/urandom | base64
来源：http://sut.hysaishi.cn

[R70] 时间戳与互转
来源：http://iqi.hnxiangtu.top

date +%s;  date -d @1700000000
来源：http://fsu.xziqi.cn

[R71] 日期格式化
来源：http://dkt.316326.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://sdj.hongshengwenyu.top

[R72] 等待端口就绪
来源：http://kar.mhx1999.top

until nc -z localhost 3306; do sleep 1; done
来源：http://cpz.yuanzhike.top

[R73] 分割大日志
来源：http://vux.birdmap.top

split -l 1000 big.log part_
来源：http://nwq.zdqjudy.top

[R74] 批量重命名
来源：http://bbu.hnqzz.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://twk.zhongyouzk.top

[R75] 导出环境变量
来源：http://bvj.pycfn.com

export PATH="$HOME/bin:$PATH"
来源：http://hfy.fktsv.cn

[R76] 使用临时文件
来源：http://mql.daxiang520.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kcs.yueranfly.top

[R77] 读取用户输入
来源：http://qms.yonumen.top

read -rp "请输入: " ans
来源：http://zal.zhaomingkeji.xyz

[R78] 交互式菜单
来源：http://tpo.jinqigfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zgu.zycfv.cn

[R79] 解析命令行选项
来源：http://ibw.xingfuxueyuan.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yuz.cashguo.top

[R80] 查看脚本执行耗时
来源：http://wnv.gzhubu.top

time ./run.sh
来源：http://cjk.yj20258888.top

================================================================================
来源：http://bwz.quarkkingdee.top

S. C / C++ 专题
来源：http://lry.shuidangran.top

================================================================================
来源：http://qnc.cashguo.top

[S01] C：Hello World
来源：http://yte.yuanzhike.top

#include <stdio.h>
来源：http://ycs.jqgfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zkc.meibo888.top

[S02] C：变量与格式化输出
来源：http://amm.guowangkeji.top

int a = 10; printf("%d\n", a);
来源：http://vmb.yangfankeji.com

[S03] C：读入整数
来源：http://cyk.zdbjq.cn

int x; scanf("%d", &x);
来源：http://pth.xuanzx.com

[S04] C：字符串复制
来源：http://rii.sxryk.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mbc.tanke756.top

[S05] C：字符串长度
来源：http://cas.wangdashe.top

strlen(s)
来源：http://jyz.ppjwa.cn

[S06] C：字符串比较
来源：http://kvt.daxiang520.top

strcmp(a, b) == 0
来源：http://veg.wangdashe.top

[S07] C：数组遍历求和
来源：http://aki.chenlongwang.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://isw.jyoumei.cn

[S08] C：动态内存分配与释放
来源：http://jfm.cucudq.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hmg.c1oappe.top

[S09] C：结构体定义与初始化
来源：http://crm.yongpay.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vzi.shuidangran.top

[S10] C：指针与解引用
来源：http://ven.cucudq.cn

int *p = &a;  *p = 5;
来源：http://fvu.jinyuanbaomall.cn

[S11] C：逐行读文件
来源：http://zhj.aibaodan.cn

FILE *f = fopen("a.txt", "r");
来源：http://tmc.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nsa.snrcjt.cn

fclose(f);
来源：http://cwu.yongpay.top

[S12] C：写文件
来源：http://dhm.9152youxi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tsu.yvedp.cn

[S13] C：宏定义
来源：http://kuf.xuetiantiany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vqx.hywenlv.cn

[S14] C：枚举
来源：http://cea.cdnleiting.top

enum Color { RED, GREEN, BLUE };
来源：http://hmb.sufxvd.cn

[S15] C：类型转换
来源：http://rfu.guannengcc.top

(double) a / b
来源：http://xjt.c1oappe.top

[S16] C：位操作置位
来源：http://dax.chenlongwang.top

x |= (1 << 3);
来源：http://kbp.smart0.xyz

[S17] C：安全拼接字符串
来源：http://wgl.zhengqikj.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pbh.xinyue.icu

[S18] C：命令行参数
来源：http://glf.yanxiufei.cn

int main(int argc, char **argv)
来源：http://aga.guannengcc.top

[S19] C：快速排序
来源：http://fop.zhiwuduotai.top

qsort(a, n, sizeof(int), cmp);
来源：http://wox.nanxuanxn.top

[S20] C：二分查找
来源：http://tgh.daxiang520.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kyi.gaohongyu789.top

[S21] C：字符类别判断
来源：http://qzn.jinqigufen.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bwu.cashguo.top

[S22] C：字符串转数字
来源：http://wjs.nanxuanxn.top

atoi("42");  strtod("3.14", NULL);
来源：http://dqu.fehbvm.com

[S23] C：随机数
来源：http://nkj.tarul.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://oqb.jyoumei.cn

[S24] C：获取本地时间
来源：http://bpt.jianghu66.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hpt.cdnleiting.top

[S25] C：内存拷贝
来源：http://npj.yueranfly.top

memcpy(dst, src, n);
来源：http://ste.jinghuilouyu.cn

[S26] C：内存清零
来源：http://ggt.cheryme.top

memset(a, 0, sizeof a);
来源：http://hbs.316326.xyz

[S27] C：定义常量
来源：http://gez.hywenlv.cn

const double PI = 3.14159;
来源：http://kns.hammf.cn

[S28] C：静态变量
来源：http://ihc.mhx1999.top

static int counter = 0;
来源：http://vml.zdbjq.cn

[S29] C：变参函数
来源：http://fmb.zhongyouzk.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qww.chenlongwang.top

[S30] C：头文件保护
来源：http://zpw.yangfankeji.com

#ifndef X_H
来源：http://xsu.cashguo.top

#define X_H
来源：http://yad.guannengcc.top

#endif
来源：http://sgh.andypj.xyz

[S31] C++：Hello World
来源：http://dvb.ydzc1.top

#include <iostream>
来源：http://sig.guowangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://yui.quarkkingdee.top

[S32] C++：字符串
来源：http://boz.bbcook.cn

std::string s = "hi";  s += "!";
来源：http://upj.xuanzx.com

[S33] C++：vector 增删
来源：http://yxa.hcnkem.com

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://teu.dianchejie.cn

[S34] C++：遍历 vector
来源：http://bjd.dianchejie.cn

for (auto &x : v) { std::cout << x; }
来源：http://kzm.hcnkem.com

[S35] C++：map
来源：http://pyz.feifeiyinyue.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://olo.ctjpmb.com

[S36] C++：unordered_map
来源：http://oim.yj20258.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uoo.zdbjq.cn

[S37] C++：set
来源：http://syr.jyoumei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uuw.jinyuanbaomall.cn

[S38] C++：排序
来源：http://cht.yj202588.top

std::sort(v.begin(), v.end());
来源：http://xkl.vehdjk.com

[S39] C++：自定义比较器排序
来源：http://oph.ydjk.org.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://loj.nanxinkj.top

[S40] C++：查找元素
来源：http://xcm.xziqi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://llk.havefunace.top

[S41] C++：类与构造函数
来源：http://wkf.zdqjudy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://soz.jinghuilouyu.cn

[S42] C++：继承与虚函数
来源：http://ajf.jqgufenzy.top

class B : public Base { public: void f() override {} };
来源：http://lnv.ydjk.org.cn

[S43] C++：智能指针
来源：http://irm.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://ugg.wangshuangyany.cn

[S44] C++：引用传参
来源：http://gjt.xylfe.cn

void inc(int &x) { ++x; }
来源：http://jag.zhijiandao.cn

[S45] C++：lambda
来源：http://yov.316326.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://cjh.xinyue.icu

[S46] C++：函数模板
来源：http://iur.yfazqb.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ics.pengpengdd.cyou

[S47] C++：结构化绑定遍历
来源：http://tjr.hywenlv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hhj.jinghuilouyu.cn

[S48] C++：逐行读文件
来源：http://gmi.iojbl.cn

std::ifstream in("a.txt");  std::string line;
来源：http://swu.zdbjq.cn

while (std::getline(in, line)) { }
来源：http://wjb.ehwqpu.com

[S49] C++：写文件
来源：http://usi.shanyushiyangtech.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cmi.yj202588.top

[S50] C++：格式化数字
来源：http://gpx.sweek.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qdv.tarul.cn

[S51] C++：显式类型转换
来源：http://hxm.fanxiaobao.xyz

static_cast<double>(a) / b
来源：http://vfx.shzxlz.cn

[S52] C++：const 与 noexcept
来源：http://eff.jyoumei.cn

int size() const noexcept { return n_; }
来源：http://htc.chenlongwang.top

[S53] C++：移动语义
来源：http://csf.zdqjudy.top

std::vector<int> w = std::move(v);
来源：http://cwh.feifeiyinyue.top

[S54] C++：异常处理
来源：http://nsi.dashuyun.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jsj.shanyushiyangkeji.top

[S55] C++：结构化绑定
来源：http://jxf.fengsongda.top

auto [a, b] = std::make_pair(1, 2);
来源：http://wil.yonumen.top

[S56] C++：optional
来源：http://xjm.9152youxi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dxb.jyoumei.cn

[S57] C++：编译期常量
来源：http://zql.nanxuanxn.top

constexpr int N = 10;
来源：http://fww.xylfe.cn

[S58] C++：命名空间
来源：http://zma.zhiwuduotai.top

namespace ns { int f() { return 1; } }
来源：http://oil.ydjk.org.cn

[S59] C++：静态断言
来源：http://yqt.9152youxi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bcg.c1oappe.top

[S60] C++：遍历并删除元素
来源：http://lhl.wangshuangyany.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://apm.hongshengwenyu.top

================================================================================
来源：http://ehz.epnwcf.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://dnf.fzhhl.top

================================================================================
来源：http://mge.ydjk.org.cn

[T01] Kotlin：Hello World
来源：http://ofx.chenlongwang.top

println("Hello")
来源：http://wrd.cucudq.cn

[T02] Kotlin：变量
来源：http://rzl.yonumen.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yuf.fehbvm.com

[T03] Kotlin：字符串模板
来源：http://pxh.cdnleiting.top

"值: $b"
来源：http://kyz.sufxvd.cn

[T04] Kotlin：空安全
来源：http://cda.xingfuxueyuan.xyz

val n: String? = null;  n?.length
来源：http://yba.tianlin.xyz


<!-- 参考信息 -->