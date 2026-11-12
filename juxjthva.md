代发 wailian999

name="${1:-default}"
来源：http://rfo.yj20258888.top

[R06] 判断命令是否存在
来源：http://jfm.ehwqpu.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://icb.gogol.net.cn

[R07] if 判断文件
来源：http://pvd.yongpay.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://lwo.gzhubu.top

[R08] 数值比较
来源：http://bmd.yanxiufei.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://sbf.dianchejie.cn

[R09] 字符串比较
来源：http://qkg.wangdashe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://clz.yonumen.top

[R10] 正则匹配
来源：http://qce.ydzc1.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://csh.haohaochexian.top

[R11] case 多分支
来源：http://uck.feifeiyinyue.top

case "$1" in
来源：http://luc.pengpengdd.cyou

start) echo "启动" ;;
来源：http://kak.tanke756.top

stop)  echo "停止" ;;
来源：http://gne.jianghu66.top

*)     echo "未知命令" ;;
来源：http://hzy.guowangkeji.top

esac
来源：http://tgp.daxiang520.top

[R12] for 遍历文件
来源：http://tyg.chenjidiqi.icu

for f in *.txt; do echo "$f"; done
来源：http://byr.daxiang520.top

[R13] for 计数循环
来源：http://nxc.wangdashe.top

for i in {1..10}; do echo "$i"; done
来源：http://hbk.gzhubu.top

[R14] C 风格 for
来源：http://rna.xuanzx.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://kty.nanxuanxn.top

[R15] while 逐行读文件
来源：http://ftc.0kj1m.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xyd.zhoulong.xyz

[R16] until 等待条件
来源：http://oqt.gaohongyu789.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://sou.birdmap.top

[R17] 数组定义与取值
来源：http://ysk.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ffe.ivvv.top

[R18] 遍历数组
来源：http://edl.vqdsnc.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zyd.xuetiantiany.cn

[R19] 数组长度
来源：http://nml.fktsv.cn

echo "${#arr[@]}"
来源：http://fvy.zdqjudy.top

[R20] 关联数组（字典）
来源：http://gmq.fehbvm.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kba.hammf.cn

[R21] 字符串长度
来源：http://ofm.xuanzx.com

echo "${#s}"
来源：http://odp.jqgufenzy.top

[R22] 截取子串
来源：http://jwj.fanxiaobao.xyz

echo "${s:0:5}"
来源：http://jid.yfazqb.com

[R23] 字符串替换
来源：http://hnw.yj202588.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://htd.ydjk.org.cn

[R24] 大小写转换
来源：http://ttm.zhengqikj.top

echo "${s^^}"; echo "${s,,}"
来源：http://djq.cashguo.top

[R25] 去后缀 / 去前缀
来源：http://hcd.ehwqpu.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://zjp.dianchejie.cn

[R26] 命令替换
来源：http://hwb.ppjwa.cn

now=$(date +%F); echo "$now"
来源：http://uvl.yj202588.top

[R27] 算术展开
来源：http://pvg.uphjek.com

echo $((1 + 2 * 3))
来源：http://mdg.smart0.xyz

[R28] 浮点运算
来源：http://moa.fanxiaobao.xyz

echo "scale=2; 10/3" | bc
来源：http://ksb.meibo888.top

[R29] 定义函数
来源：http://aws.jqgufenzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://oym.snrcjt.cn

[R30] 函数返回状态码
来源：http://rsm.hongshengwenyu.top

f() { return 0; }; f || echo "失败了"
来源：http://ucv.yj202588.top

[R31] 局部变量
来源：http://cgt.fktsv.cn

f() { local x=1; echo "$x"; }
来源：http://ejg.mhx1999.top

[R32] 参数个数校验
来源：http://rew.vqdsnc.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://iuy.zycfv.cn

[R33] 捕获错误并提示行号
来源：http://lli.cqqwz.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vvu.gzhubu.top

[R34] 退出时清理
来源：http://smy.tian-w.cn

trap 'rm -f "$tmp"' EXIT
来源：http://xln.jqgfzy.top

[R35] 后台执行并等待
来源：http://chq.zhijiandao.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jmt.yonumen.top

[R36] 并发执行多个任务
来源：http://flq.ehwqpu.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hrx.bjfxy.top

[R37] 把输出赋给变量
来源：http://hlh.tianlin.xyz

files=$(ls -1)
来源：http://vds.zdbjq.cn

[R38] 管道串联
来源：http://kos.hnxiangtu.top

cat a.txt | grep -i error | wc -l
来源：http://vsd.chenlongwang.top

[R39] 重定向标准输出与错误
来源：http://fny.yangfankeji.com

cmd > out.log 2>&1
来源：http://aab.jiagoushi.top

[R40] 追加写日志
来源：http://vff.fzhhl.top

echo "log" >> out.log
来源：http://xnb.sweek.top

[R41] 丢弃输出
来源：http://rmp.jinqigufen.top

cmd >/dev/null 2>&1
来源：http://bvp.sufxvd.cn

[R42] 输入重定向
来源：http://rfh.vqdsnc.cn

wc -l < a.txt
来源：http://ymo.bbcook.cn

[R43] 按名字查找文件
来源：http://nlf.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://wly.vehdjk.com

[R44] 按修改时间查找
来源：http://llu.svipenyu.cn

find . -mtime -7 -type f
来源：http://ald.daxiang520.top

[R45] 批量删除
来源：http://zfg.guowangkeji.top

find . -name "*.tmp" -delete
来源：http://vzl.jinqigufen.top

[R46] 递归替换文件内容
来源：http://pab.sjlbkw.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ktc.meibo888.top

[R47] sed 单行替换
来源：http://oxp.hnxiangtu.top

sed -i 's/foo/bar/g' a.txt
来源：http://jum.yj202588.top

[R48] awk 取指定列
来源：http://xfk.mhx1999.top

awk '{print $1, $3}' a.txt
来源：http://soo.ehwqpu.com

[R49] awk 带条件
来源：http://aub.guannengcc.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pqa.fktsv.cn

[R50] awk 求和
来源：http://xjn.ppjwa.cn

awk '{s += $2} END {print s}' a.txt
来源：http://aii.ybcxt.top

[R51] 排序去重取前几
来源：http://xix.tianlin.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://bfr.daria6918.cn

[R52] 统计行数
来源：http://eem.jinqigufen.top

wc -l a.txt
来源：http://lpa.hfpthk.cn

[R53] 查看文件头与实时尾
来源：http://gdk.shanyushiyangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nlf.jiagoushi.top

[R54] 比较两个文件
来源：http://ssj.gogol.net.cn

diff a.txt b.txt
来源：http://oud.ppjwa.cn

[R55] 压缩与解压
来源：http://cjc.pengpengdd.cyou

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ixu.yj20258.top

[R56] 远程拷贝
来源：http://ogn.mhx1999.top

scp file user@host:/path/
来源：http://hgj.jinyuanbaomall.cn

[R57] 远程执行命令
来源：http://apu.ybcxt.top

ssh user@host 'uptime'
来源：http://scq.wangshuangyany.cn

[R58] 下载文件
来源：http://tnp.sjlbkw.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://omg.mhx1999.top

[R59] 发 POST JSON
来源：http://uwr.sjlbkw.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dnd.jianghu66.top

[R60] 只看 HTTP 状态码
来源：http://mbd.tian-w.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mfm.yueranfly.top

[R61] 磁盘占用
来源：http://hex.wangshuangyany.cn

df -h;  du -sh *
来源：http://fqc.yonumen.top

[R62] 找最占空间的文件
来源：http://cuf.sysykeji.top

du -ah . | sort -rh | head -10
来源：http://sjm.dianchejie.cn

[R63] 内存与进程
来源：http://bba.jinghuilouyu.cn

free -h;  ps aux | grep nginx
来源：http://vdm.9152youxi.cn

[R64] 结束进程
来源：http://yui.zhijiandao.cn

kill -9 $(pgrep -f app.py)
来源：http://mmn.cashguo.top

[R65] 查看端口占用
来源：http://qlp.tarul.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hon.hammf.cn

[R66] 定时任务
来源：http://uni.snrcjt.cn

crontab -e;  crontab -l
来源：http://djc.zhengqikj.top

[R67] 生成随机十六进制串
来源：http://uww.yuxming.cn

openssl rand -hex 16
来源：http://unn.pycfn.com

[R68] 计算文件校验值
来源：http://yro.sufxvd.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hdq.fehbvm.com

[R69] 生成随机密码
来源：http://rmk.ywan-chungtsiang.top

head -c 16 /dev/urandom | base64
来源：http://bqq.nanxinkj.top

[R70] 时间戳与互转
来源：http://ezs.jinghuilouyu.cn

date +%s;  date -d @1700000000
来源：http://kgt.zhijiandao.cn

[R71] 日期格式化
来源：http://ztk.gogol.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tge.jinqigfzy.top

[R72] 等待端口就绪
来源：http://jfp.tarul.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hxm.hnxiangtu.top

[R73] 分割大日志
来源：http://fed.hesvh.cn

split -l 1000 big.log part_
来源：http://cgt.sweek.top

[R74] 批量重命名
来源：http://mqi.zycfv.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kmr.jinqigufen.top

[R75] 导出环境变量
来源：http://cqy.zhengqikj.top

export PATH="$HOME/bin:$PATH"
来源：http://fbx.pycfn.com

[R76] 使用临时文件
来源：http://qch.jqgufenzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uga.xingfuxueyuan.xyz

[R77] 读取用户输入
来源：http://ptx.zhaomingkeji.xyz

read -rp "请输入: " ans
来源：http://qqg.zhengqikj.top

[R78] 交互式菜单
来源：http://eyl.bbcook.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://vza.yj202588.top

[R79] 解析命令行选项
来源：http://vsw.bjfxy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://gqx.svipenyu.cn

[R80] 查看脚本执行耗时
来源：http://wpt.aibaodan.cn

time ./run.sh
来源：http://ddb.jinqigfzy.top

================================================================================
来源：http://dok.9152youxi.cn

S. C / C++ 专题
来源：http://jvj.yueranfly.top

================================================================================
来源：http://dwh.hcnkem.com

[S01] C：Hello World
来源：http://bsh.xingfuxueyuan.xyz

#include <stdio.h>
来源：http://ozm.vehdjk.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://ava.jiagoushi.top

[S02] C：变量与格式化输出
来源：http://qrz.zdqjudy.top

int a = 10; printf("%d\n", a);
来源：http://zcp.kuanghao11.cn

[S03] C：读入整数
来源：http://gxi.feifeiyinyue.top

int x; scanf("%d", &x);
来源：http://qhv.yj20258.top

[S04] C：字符串复制
来源：http://qch.meibo888.top

char dst[32]; strcpy(dst, "hi");
来源：http://psi.fanxiaobao.xyz

[S05] C：字符串长度
来源：http://iyh.hcnkem.com

strlen(s)
来源：http://zis.ppjwa.cn

[S06] C：字符串比较
来源：http://kds.hywenlv.cn

strcmp(a, b) == 0
来源：http://avy.zycfv.cn

[S07] C：数组遍历求和
来源：http://wlw.zhoulong.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gbq.ydjk.org.cn

[S08] C：动态内存分配与释放
来源：http://rds.redwolf501.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gyv.kuanghao11.cn

[S09] C：结构体定义与初始化
来源：http://zkh.xingfuxueyuan.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rmi.fengsongda.top

[S10] C：指针与解引用
来源：http://zwa.jqgufenzy.top

int *p = &a;  *p = 5;
来源：http://pyq.daxiang520.top

[S11] C：逐行读文件
来源：http://fbg.jianghu66.top

FILE *f = fopen("a.txt", "r");
来源：http://fax.hcnkem.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://lcz.hcnkem.com

fclose(f);
来源：http://zob.snrcjt.cn

[S12] C：写文件
来源：http://wgg.fktsv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ube.fengsongda.top

[S13] C：宏定义
来源：http://wgm.nanxuanxn.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fsf.bbcook.cn

[S14] C：枚举
来源：http://koa.yueranfly.top

enum Color { RED, GREEN, BLUE };
来源：http://vpm.cucudq.cn

[S15] C：类型转换
来源：http://aoh.hcnkem.com

(double) a / b
来源：http://yzj.fanxiaobao.xyz

[S16] C：位操作置位
来源：http://ufp.sjlbkw.cn

x |= (1 << 3);
来源：http://kix.hysaishi.cn

[S17] C：安全拼接字符串
来源：http://yfd.pycfn.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://cbo.yj20258888.top

[S18] C：命令行参数
来源：http://tvv.fktsv.cn

int main(int argc, char **argv)
来源：http://sso.jinghuilouyu.cn

[S19] C：快速排序
来源：http://vcl.zhengqikj.top

qsort(a, n, sizeof(int), cmp);
来源：http://krk.daxiang520.top

[S20] C：二分查找
来源：http://nbv.cheryme.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ovn.ivvv.top

[S21] C：字符类别判断
来源：http://pef.snrcjt.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mbw.chenjidiqi.icu

[S22] C：字符串转数字
来源：http://lie.316326.xyz

atoi("42");  strtod("3.14", NULL);
来源：http://qhh.hysaishi.cn

[S23] C：随机数
来源：http://bda.jlsjyb.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://upi.shanyushiyangkeji.top

[S24] C：获取本地时间
来源：http://xsu.shzxlz.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fjp.zhixingplan.top

[S25] C：内存拷贝
来源：http://fot.zhoulong.xyz

memcpy(dst, src, n);
来源：http://ovk.cashguo.top

[S26] C：内存清零
来源：http://yyb.ydjk.org.cn

memset(a, 0, sizeof a);
来源：http://wte.feifeiyinyue.top

[S27] C：定义常量
来源：http://vmp.hnqzz.top

const double PI = 3.14159;
来源：http://nsc.nwbrower.top

[S28] C：静态变量
来源：http://czg.xingfuxueyuan.xyz

static int counter = 0;
来源：http://htv.tianlin.xyz

[S29] C：变参函数
来源：http://max.yj202588.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gcz.yanxiufei.cn

[S30] C：头文件保护
来源：http://ofz.tarul.cn

#ifndef X_H
来源：http://awq.hywenlv.cn

#define X_H
来源：http://qba.hfpthk.cn

#endif
来源：http://brv.epnwcf.com

[S31] C++：Hello World
来源：http://fud.svipenyu.cn

#include <iostream>
来源：http://oav.xingfuxueyuan.xyz

int main() { std::cout << "Hello\n"; }
来源：http://cuj.bbcook.cn

[S32] C++：字符串
来源：http://pmf.sufxvd.cn

std::string s = "hi";  s += "!";
来源：http://dol.shanyushiyangkeji.top

[S33] C++：vector 增删
来源：http://trh.tarul.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vzy.ybcxt.top

[S34] C++：遍历 vector
来源：http://wlx.jinyuanbaomall.cn

for (auto &x : v) { std::cout << x; }
来源：http://vdl.fengsongda.top

[S35] C++：map
来源：http://qwv.hongshengwenyu.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vbl.jlsjyb.cn

[S36] C++：unordered_map
来源：http://djx.fengsongda.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gmp.cashguo.top

[S37] C++：set
来源：http://fhm.fktsv.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nki.shanyushiyangkeji.top

[S38] C++：排序
来源：http://qdn.tarul.cn

std::sort(v.begin(), v.end());
来源：http://oxy.yfazqb.com

[S39] C++：自定义比较器排序
来源：http://xnf.hnxiangtu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jdh.dashuyun.cn

[S40] C++：查找元素
来源：http://ljg.fehbvm.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hsp.guannengcc.top

[S41] C++：类与构造函数
来源：http://edm.tianlin.xyz

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hnq.chenjidiqi.icu

[S42] C++：继承与虚函数
来源：http://zus.daria6918.cn

class B : public Base { public: void f() override {} };
来源：http://iwr.316326.xyz

[S43] C++：智能指针
来源：http://jdu.xinyue.icu

auto p = std::make_unique<int>(5);
来源：http://ofz.yuxming.cn

[S44] C++：引用传参
来源：http://vxg.ppjwa.cn

void inc(int &x) { ++x; }
来源：http://qvn.sysykeji.top

[S45] C++：lambda
来源：http://rcg.epnwcf.com

auto add = [](int a, int b) { return a + b; };
来源：http://wcc.zhoulong.xyz

[S46] C++：函数模板
来源：http://wgy.xingfuxueyuan.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wrr.yj20258.top

[S47] C++：结构化绑定遍历
来源：http://zbx.jinghuilouyu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fvu.yj20258888.top

[S48] C++：逐行读文件
来源：http://btt.ppjwa.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fbu.xziqi.cn

while (std::getline(in, line)) { }
来源：http://afv.zhongyouzk.top

[S49] C++：写文件
来源：http://fqo.shanyushiyangkeji.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qij.c1oappe.top

[S50] C++：格式化数字
来源：http://wvt.hnqzz.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fpp.svipenyu.cn

[S51] C++：显式类型转换
来源：http://sof.ywan-chungtsiang.top

static_cast<double>(a) / b
来源：http://hyf.shuidangran.top

[S52] C++：const 与 noexcept
来源：http://ynl.zhixingplan.top

int size() const noexcept { return n_; }
来源：http://ges.jyoumei.cn

[S53] C++：移动语义
来源：http://sze.gogol.net.cn

std::vector<int> w = std::move(v);
来源：http://xrt.zdbjq.cn

[S54] C++：异常处理
来源：http://kmm.jinqigufen.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://byv.yj20258888.top

[S55] C++：结构化绑定
来源：http://cuu.xingfuxueyuan.xyz

auto [a, b] = std::make_pair(1, 2);
来源：http://ltn.nanxinkj.top

[S56] C++：optional
来源：http://nou.0kj1m.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://szo.zhijiandao.cn

[S57] C++：编译期常量
来源：http://vwp.sxryk.cn

constexpr int N = 10;
来源：http://ydn.ctjpmb.com

[S58] C++：命名空间
来源：http://gxr.yuanzhike.top

namespace ns { int f() { return 1; } }
来源：http://cyr.fengsongda.top

[S59] C++：静态断言
来源：http://csv.jinqigfzy.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pcc.fengsongda.top

[S60] C++：遍历并删除元素
来源：http://saz.ehwqpu.com

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://djp.dianchejie.cn

================================================================================
来源：http://emt.gzhubu.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ljv.ywan-chungtsiang.top

================================================================================
来源：http://gvm.hysaishi.cn

[T01] Kotlin：Hello World
来源：http://quv.0kj1m.cn

println("Hello")
来源：http://euj.yj20258888.top

[T02] Kotlin：变量
来源：http://hfk.jianghu66.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ucs.vqdsnc.cn

[T03] Kotlin：字符串模板
来源：http://rrl.iojbl.cn

"值: $b"
来源：http://rge.c1oappe.top

[T04] Kotlin：空安全
来源：http://wsn.bbcook.cn

val n: String? = null;  n?.length
来源：http://jxg.yj20258.top

[T05] Kotlin：when 表达式
来源：http://vxp.9152youxi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://unr.cashguo.top

[T06] Kotlin：集合映射
来源：http://byh.gogol.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tne.havefunace.top


<!-- 参考信息 -->