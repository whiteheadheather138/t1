代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dxa.yj20258888.top

[R08] 数值比较
来源：http://hmx.aibaodan.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dnu.zhijiandao.cn

[R09] 字符串比较
来源：http://rqk.iojbl.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://juz.guannengcc.top

[R10] 正则匹配
来源：http://ocb.hesvh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mbx.yfazqb.com

[R11] case 多分支
来源：http://uwl.vehdjk.com

case "$1" in
来源：http://ceq.pycfn.com

start) echo "启动" ;;
来源：http://hrm.gogol.net.cn

stop)  echo "停止" ;;
来源：http://jaw.jyoumei.cn

*)     echo "未知命令" ;;
来源：http://ixe.hysaishi.cn

esac
来源：http://nnr.hongshengwenyu.top

[R12] for 遍历文件
来源：http://sqj.jinghuilouyu.cn

for f in *.txt; do echo "$f"; done
来源：http://izf.daxiang520.top

[R13] for 计数循环
来源：http://udu.jlsjyb.cn

for i in {1..10}; do echo "$i"; done
来源：http://vgk.hongshengwenyu.top

[R14] C 风格 for
来源：http://ikh.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rzh.jlsjyb.cn

[R15] while 逐行读文件
来源：http://taw.daxiang520.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fgt.ydzc1.top

[R16] until 等待条件
来源：http://tbn.hfpthk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://svu.wangdashe.top

[R17] 数组定义与取值
来源：http://ukm.jinqigufen.top

arr=(a b c); echo "${arr[0]}"
来源：http://anz.yfazqb.com

[R18] 遍历数组
来源：http://whc.ydzc1.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://nmx.yj20258888.top

[R19] 数组长度
来源：http://waw.fehbvm.com

echo "${#arr[@]}"
来源：http://wgm.guowangkeji.top

[R20] 关联数组（字典）
来源：http://wjl.mhx1999.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://umn.zhixingplan.top

[R21] 字符串长度
来源：http://ree.smart0.xyz

echo "${#s}"
来源：http://cuc.epnwcf.com

[R22] 截取子串
来源：http://swv.jiagoushi.top

echo "${s:0:5}"
来源：http://zjw.yongpay.top

[R23] 字符串替换
来源：http://kng.daxiang520.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bvj.ivvv.top

[R24] 大小写转换
来源：http://wyn.gotoacloud.top

echo "${s^^}"; echo "${s,,}"
来源：http://vxr.yvedp.cn

[R25] 去后缀 / 去前缀
来源：http://heh.aizwys.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xcu.ydjk.org.cn

[R26] 命令替换
来源：http://xqx.nanxinkj.top

now=$(date +%F); echo "$now"
来源：http://nyb.dianchejie.cn

[R27] 算术展开
来源：http://eye.dashuyun.cn

echo $((1 + 2 * 3))
来源：http://ujw.bjfxy.top

[R28] 浮点运算
来源：http://qvp.dianchejie.cn

echo "scale=2; 10/3" | bc
来源：http://vuq.gogol.net.cn

[R29] 定义函数
来源：http://lqj.wangdashe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ayx.dianchejie.cn

[R30] 函数返回状态码
来源：http://wjj.aizwys.cn

f() { return 0; }; f || echo "失败了"
来源：http://sbr.zhongyouzk.top

[R31] 局部变量
来源：http://kne.iojbl.cn

f() { local x=1; echo "$x"; }
来源：http://kph.pycfn.com

[R32] 参数个数校验
来源：http://ucd.tanke756.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tit.yueranfly.top

[R33] 捕获错误并提示行号
来源：http://rhm.zhijiandao.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sad.52xcode.cn

[R34] 退出时清理
来源：http://hli.zhengqikj.top

trap 'rm -f "$tmp"' EXIT
来源：http://ala.ywan-chungtsiang.top

[R35] 后台执行并等待
来源：http://cqy.smart0.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://hnx.dianchejie.cn

[R36] 并发执行多个任务
来源：http://zbw.shangyingyoupin.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vct.fanxiaobao.xyz

[R37] 把输出赋给变量
来源：http://qcm.birdmap.top

files=$(ls -1)
来源：http://vvu.nanxuanxn.top

[R38] 管道串联
来源：http://mce.hysaishi.cn

cat a.txt | grep -i error | wc -l
来源：http://fwf.xuanzx.com

[R39] 重定向标准输出与错误
来源：http://guw.snrcjt.cn

cmd > out.log 2>&1
来源：http://mjq.jinqigufen.top

[R40] 追加写日志
来源：http://rzt.tarul.cn

echo "log" >> out.log
来源：http://yyl.ydzc1.top

[R41] 丢弃输出
来源：http://sye.cashguo.top

cmd >/dev/null 2>&1
来源：http://vsg.yvedp.cn

[R42] 输入重定向
来源：http://axz.xziqi.cn

wc -l < a.txt
来源：http://edn.ydzc1.top

[R43] 按名字查找文件
来源：http://swg.yfazqb.com

find . -name "*.log" -type f
来源：http://ahp.zhiwuduotai.top

[R44] 按修改时间查找
来源：http://vxa.mhx1999.top

find . -mtime -7 -type f
来源：http://cnr.gotoacloud.top

[R45] 批量删除
来源：http://zeq.gogol.net.cn

find . -name "*.tmp" -delete
来源：http://rmd.wangdashe.top

[R46] 递归替换文件内容
来源：http://arb.bbcook.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://skt.nanxinkj.top

[R47] sed 单行替换
来源：http://ady.vqdsnc.cn

sed -i 's/foo/bar/g' a.txt
来源：http://kig.vehdjk.com

[R48] awk 取指定列
来源：http://iyd.birdmap.top

awk '{print $1, $3}' a.txt
来源：http://dti.guannengcc.top

[R49] awk 带条件
来源：http://nwm.ywan-chungtsiang.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mgq.zhaomingkeji.xyz

[R50] awk 求和
来源：http://rfx.fengsongda.top

awk '{s += $2} END {print s}' a.txt
来源：http://fds.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://kum.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://eho.cheryme.top

[R52] 统计行数
来源：http://axs.pycfn.com

wc -l a.txt
来源：http://wtg.ehwqpu.com

[R53] 查看文件头与实时尾
来源：http://yoi.gotoacloud.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://goe.aizwys.cn

[R54] 比较两个文件
来源：http://awu.epnwcf.com

diff a.txt b.txt
来源：http://dxy.jiagoushi.top

[R55] 压缩与解压
来源：http://keu.xuetiantiany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://svw.fehbvm.com

[R56] 远程拷贝
来源：http://ppp.svipenyu.cn

scp file user@host:/path/
来源：http://nlk.smart0.xyz

[R57] 远程执行命令
来源：http://fji.daxiang520.top

ssh user@host 'uptime'
来源：http://ilq.redwolf501.top

[R58] 下载文件
来源：http://ejn.jinqigufen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vzb.gaohongyu789.top

[R59] 发 POST JSON
来源：http://wdv.jianghu66.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bxh.uphjek.com

[R60] 只看 HTTP 状态码
来源：http://fpd.gzhubu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yyq.cashguo.top

[R61] 磁盘占用
来源：http://taa.shangyingyoupin.top

df -h;  du -sh *
来源：http://ipb.pycfn.com

[R62] 找最占空间的文件
来源：http://wxo.zdbjq.cn

du -ah . | sort -rh | head -10
来源：http://aei.guannengcc.top

[R63] 内存与进程
来源：http://bna.hammf.cn

free -h;  ps aux | grep nginx
来源：http://xel.jinghuilouyu.cn

[R64] 结束进程
来源：http://ntf.redwolf501.top

kill -9 $(pgrep -f app.py)
来源：http://awk.aizwys.cn

[R65] 查看端口占用
来源：http://pad.yanxiufei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ukx.pengpengdd.cyou

[R66] 定时任务
来源：http://ybl.wangshuangyany.cn

crontab -e;  crontab -l
来源：http://wew.gotoacloud.top

[R67] 生成随机十六进制串
来源：http://dqo.9152youxi.cn

openssl rand -hex 16
来源：http://clf.xinyue.icu

[R68] 计算文件校验值
来源：http://njn.aizwys.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xtj.zhengqikj.top

[R69] 生成随机密码
来源：http://yae.tanke756.top

head -c 16 /dev/urandom | base64
来源：http://evc.tian-w.cn

[R70] 时间戳与互转
来源：http://ebg.jyoumei.cn

date +%s;  date -d @1700000000
来源：http://ipt.ydzc1.top

[R71] 日期格式化
来源：http://mtg.vqdsnc.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dtw.redwolf501.top

[R72] 等待端口就绪
来源：http://jmp.haohaochexian.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ldu.sxryk.cn

[R73] 分割大日志
来源：http://tqj.bbcook.cn

split -l 1000 big.log part_
来源：http://fur.haohaochexian.top

[R74] 批量重命名
来源：http://mng.shanyushiyangkeji.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yqh.jqgufenzy.top

[R75] 导出环境变量
来源：http://fzv.jinqigufen.top

export PATH="$HOME/bin:$PATH"
来源：http://xax.fktsv.cn

[R76] 使用临时文件
来源：http://wrv.tarul.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lom.sweek.top

[R77] 读取用户输入
来源：http://htc.nwbrower.top

read -rp "请输入: " ans
来源：http://apw.hysaishi.cn

[R78] 交互式菜单
来源：http://ghk.cdnleiting.top

select opt in a b c; do echo "$opt"; break; done
来源：http://duu.ivvv.top

[R79] 解析命令行选项
来源：http://uef.9152youxi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zvz.jlsjyb.cn

[R80] 查看脚本执行耗时
来源：http://muy.birdmap.top

time ./run.sh
来源：http://uso.pycfn.com

================================================================================
来源：http://zwz.hywenlv.cn

S. C / C++ 专题
来源：http://tmn.yanxiufei.cn

================================================================================
来源：http://zpv.316326.xyz

[S01] C：Hello World
来源：http://ecg.wangdashe.top

#include <stdio.h>
来源：http://nsw.gaohongyu789.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://dzo.shanyushiyangtech.top

[S02] C：变量与格式化输出
来源：http://mco.redwolf501.top

int a = 10; printf("%d\n", a);
来源：http://jnk.fehbvm.com

[S03] C：读入整数
来源：http://asr.kuanghao11.cn

int x; scanf("%d", &x);
来源：http://few.bbcook.cn

[S04] C：字符串复制
来源：http://usr.fengsongda.top

char dst[32]; strcpy(dst, "hi");
来源：http://dub.yj20258888.top

[S05] C：字符串长度
来源：http://ejb.guannengcc.top

strlen(s)
来源：http://rho.uphjek.com

[S06] C：字符串比较
来源：http://pag.hywenlv.cn

strcmp(a, b) == 0
来源：http://sif.cashguo.top

[S07] C：数组遍历求和
来源：http://wdb.birdmap.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eba.jlsjyb.cn

[S08] C：动态内存分配与释放
来源：http://ilc.ybcxt.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qla.wangshuangyany.cn

[S09] C：结构体定义与初始化
来源：http://zoi.fehbvm.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://viw.sufxvd.cn

[S10] C：指针与解引用
来源：http://euw.bbcook.cn

int *p = &a;  *p = 5;
来源：http://kdp.yvedp.cn

[S11] C：逐行读文件
来源：http://ruy.cdnleiting.top

FILE *f = fopen("a.txt", "r");
来源：http://nvx.tianlin.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://ffi.tanke756.top

fclose(f);
来源：http://tvm.hammf.cn

[S12] C：写文件
来源：http://qwk.ivvv.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://csk.daxiang520.top

[S13] C：宏定义
来源：http://yfj.nanxuanxn.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://iqf.gzhubu.top

[S14] C：枚举
来源：http://llm.quarkkingdee.top

enum Color { RED, GREEN, BLUE };
来源：http://ece.hnqzz.top

[S15] C：类型转换
来源：http://vsl.yj202588.top

(double) a / b
来源：http://rin.cashguo.top

[S16] C：位操作置位
来源：http://iaf.xylfe.cn

x |= (1 << 3);
来源：http://tzw.tanke756.top

[S17] C：安全拼接字符串
来源：http://tyt.snrcjt.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dvz.yj20258.top

[S18] C：命令行参数
来源：http://coj.tanke756.top

int main(int argc, char **argv)
来源：http://mgm.vehdjk.com

[S19] C：快速排序
来源：http://lxt.xziqi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gpv.hammf.cn

[S20] C：二分查找
来源：http://eag.zhiwuduotai.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hwm.hnqzz.top

[S21] C：字符类别判断
来源：http://pvw.hywenlv.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pjy.sufxvd.cn

[S22] C：字符串转数字
来源：http://vai.sysykeji.top

atoi("42");  strtod("3.14", NULL);
来源：http://hnt.daria6918.cn

[S23] C：随机数
来源：http://skq.bjfxy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://luc.yfazqb.com

[S24] C：获取本地时间
来源：http://ulx.zhongyouzk.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rkt.xziqi.cn

[S25] C：内存拷贝
来源：http://ues.dashuyun.cn

memcpy(dst, src, n);
来源：http://sjh.hnqzz.top

[S26] C：内存清零
来源：http://ply.0kj1m.cn

memset(a, 0, sizeof a);
来源：http://rmn.cqqwz.cn

[S27] C：定义常量
来源：http://ter.bjfxy.top

const double PI = 3.14159;
来源：http://bur.zhengqikj.top

[S28] C：静态变量
来源：http://emv.smart0.xyz

static int counter = 0;
来源：http://awc.fzhhl.top

[S29] C：变参函数
来源：http://sea.tanke756.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://era.c1oappe.top

[S30] C：头文件保护
来源：http://cfo.9152youxi.cn

#ifndef X_H
来源：http://fic.ctjpmb.com

#define X_H
来源：http://xwy.yvedp.cn

#endif
来源：http://mej.ehwqpu.com

[S31] C++：Hello World
来源：http://mhk.yangfankeji.com

#include <iostream>
来源：http://fjy.shanyushiyangtech.top

int main() { std::cout << "Hello\n"; }
来源：http://ufk.vehdjk.com

[S32] C++：字符串
来源：http://sgi.sjlbkw.cn

std::string s = "hi";  s += "!";
来源：http://jeg.nwbrower.top

[S33] C++：vector 增删
来源：http://beu.zhengqikj.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://flg.hcnkem.com

[S34] C++：遍历 vector
来源：http://qqu.daria6918.cn

for (auto &x : v) { std::cout << x; }
来源：http://ssr.hcnkem.com

[S35] C++：map
来源：http://eru.sysykeji.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xga.fktsv.cn

[S36] C++：unordered_map
来源：http://qzf.52xcode.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://odw.zdqjudy.top

[S37] C++：set
来源：http://nos.yanxiufei.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jvq.daria6918.cn

[S38] C++：排序
来源：http://skv.gotoacloud.top

std::sort(v.begin(), v.end());
来源：http://xri.jqgufenzy.top

[S39] C++：自定义比较器排序
来源：http://roa.zhongyouzk.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hsa.zdbjq.cn

[S40] C++：查找元素
来源：http://fgs.yuanzhike.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ymy.ppjwa.cn

[S41] C++：类与构造函数
来源：http://fos.zhongyouzk.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nwp.tanke756.top

[S42] C++：继承与虚函数
来源：http://aaw.sjlbkw.cn

class B : public Base { public: void f() override {} };
来源：http://vig.havefunace.top

[S43] C++：智能指针
来源：http://mwj.chenjidiqi.icu

auto p = std::make_unique<int>(5);
来源：http://kcq.jinqigfzy.top

[S44] C++：引用传参
来源：http://wsz.zdbjq.cn

void inc(int &x) { ++x; }
来源：http://awg.zhixingplan.top

[S45] C++：lambda
来源：http://vqb.9152youxi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bvl.svipenyu.cn

[S46] C++：函数模板
来源：http://tjf.yvedp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hnx.tarul.cn

[S47] C++：结构化绑定遍历
来源：http://ozr.zycfv.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ala.tianlin.xyz

[S48] C++：逐行读文件
来源：http://rrn.hnxiangtu.top

std::ifstream in("a.txt");  std::string line;
来源：http://kuw.snrcjt.cn

while (std::getline(in, line)) { }
来源：http://sec.cheryme.top

[S49] C++：写文件
来源：http://byt.0kj1m.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rwb.haohaochexian.top

[S50] C++：格式化数字
来源：http://rov.wangdashe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pku.shangyingyoupin.top

[S51] C++：显式类型转换
来源：http://fku.hammf.cn

static_cast<double>(a) / b
来源：http://pyv.jinqigfzy.top

[S52] C++：const 与 noexcept
来源：http://xrc.cqqwz.cn

int size() const noexcept { return n_; }
来源：http://fhy.sjlbkw.cn

[S53] C++：移动语义
来源：http://ghq.gogol.net.cn

std::vector<int> w = std::move(v);
来源：http://ufy.cucudq.cn

[S54] C++：异常处理
来源：http://vdp.andypj.xyz

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://djg.vehdjk.com

[S55] C++：结构化绑定
来源：http://wjm.redwolf501.top

auto [a, b] = std::make_pair(1, 2);
来源：http://agr.snrcjt.cn

[S56] C++：optional
来源：http://akb.shzxlz.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aek.snrcjt.cn

[S57] C++：编译期常量
来源：http://fip.yj202588.top

constexpr int N = 10;
来源：http://epi.tian-w.cn

[S58] C++：命名空间
来源：http://sjp.fanxiaobao.xyz

namespace ns { int f() { return 1; } }
来源：http://sbh.c1oappe.top

[S59] C++：静态断言
来源：http://xrz.andypj.xyz

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xmb.zhijiandao.cn

[S60] C++：遍历并删除元素
来源：http://yib.hnqzz.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kgw.snrcjt.cn

================================================================================
来源：http://zwp.vehdjk.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lkc.tian-w.cn

================================================================================
来源：http://gop.tanke756.top

[T01] Kotlin：Hello World
来源：http://yjo.pengpengdd.cyou

println("Hello")
来源：http://pqp.xziqi.cn

[T02] Kotlin：变量
来源：http://ebv.zhoulong.xyz

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://gqs.ydzc1.top

[T03] Kotlin：字符串模板
来源：http://ppd.aibaodan.cn

"值: $b"
来源：http://hec.tianlin.xyz

[T04] Kotlin：空安全
来源：http://htd.fanxiaobao.xyz

val n: String? = null;  n?.length
来源：http://gon.pycfn.com

[T05] Kotlin：when 表达式
来源：http://soy.mhx1999.top

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gvp.daxiang520.top

[T06] Kotlin：集合映射
来源：http://yfo.smart0.xyz

listOf(1, 2, 3).map { it * 2 }
来源：http://hat.shuidangran.top

[T07] Kotlin：集合过滤
来源：http://vdq.vehdjk.com

listOf(1, 2, 3).filter { it > 1 }
来源：http://yys.vqdsnc.cn

[T08] Kotlin：数据类
来源：http://bxz.jiagoushi.top

data class User(val name: String, val age: Int)
来源：http://bso.yj20258.top


<!-- 参考信息 -->