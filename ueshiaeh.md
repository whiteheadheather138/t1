代发 wailian999

esac
来源：http://mqo.zhoulong.xyz

[R12] for 遍历文件
来源：http://nqs.jinqigfzy.top

for f in *.txt; do echo "$f"; done
来源：http://rmb.fanxiaobao.xyz

[R13] for 计数循环
来源：http://aor.ydzc1.top

for i in {1..10}; do echo "$i"; done
来源：http://ije.jianghu66.top

[R14] C 风格 for
来源：http://kdl.jqgfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wzd.kuanghao11.cn

[R15] while 逐行读文件
来源：http://rkx.fehbvm.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ffs.gotoacloud.top

[R16] until 等待条件
来源：http://cqt.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://che.haohaochexian.top

[R17] 数组定义与取值
来源：http://tzh.andypj.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://oav.fzhhl.top

[R18] 遍历数组
来源：http://rlx.zhiwuduotai.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://dgq.birdmap.top

[R19] 数组长度
来源：http://vxk.daria6918.cn

echo "${#arr[@]}"
来源：http://cwj.shzxlz.cn

[R20] 关联数组（字典）
来源：http://shg.hywenlv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ycw.vehdjk.com

[R21] 字符串长度
来源：http://jkf.chenzaomai.com

echo "${#s}"
来源：http://wyw.yanxiufei.cn

[R22] 截取子串
来源：http://hvu.daxiang520.top

echo "${s:0:5}"
来源：http://rkv.hnxiangtu.top

[R23] 字符串替换
来源：http://vgx.wangdashe.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jcc.sweek.top

[R24] 大小写转换
来源：http://xdt.yuanzhike.top

echo "${s^^}"; echo "${s,,}"
来源：http://yft.jianghu66.top

[R25] 去后缀 / 去前缀
来源：http://ovi.quarkkingdee.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ljl.hammf.cn

[R26] 命令替换
来源：http://hgn.snrcjt.cn

now=$(date +%F); echo "$now"
来源：http://vgm.ppjwa.cn

[R27] 算术展开
来源：http://tln.zhengqikj.top

echo $((1 + 2 * 3))
来源：http://nge.yuanzhike.top

[R28] 浮点运算
来源：http://jpb.jyoumei.cn

echo "scale=2; 10/3" | bc
来源：http://sfj.jinqigfzy.top

[R29] 定义函数
来源：http://evq.jyoumei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ikd.zhoulong.xyz

[R30] 函数返回状态码
来源：http://zuv.wangshuangyany.cn

f() { return 0; }; f || echo "失败了"
来源：http://zqn.zdqjudy.top

[R31] 局部变量
来源：http://wkb.zhongyouzk.top

f() { local x=1; echo "$x"; }
来源：http://dxr.yongpay.top

[R32] 参数个数校验
来源：http://tqj.iojbl.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zoc.yanxiufei.cn

[R33] 捕获错误并提示行号
来源：http://cmo.zdqjudy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uef.yuxming.cn

[R34] 退出时清理
来源：http://tjy.nanxuanxn.top

trap 'rm -f "$tmp"' EXIT
来源：http://quc.nanxuanxn.top

[R35] 后台执行并等待
来源：http://tqw.jianghu66.top

sleep 5 & pid=$!; wait "$pid"
来源：http://sbp.chenlongwang.top

[R36] 并发执行多个任务
来源：http://kdn.daxiang520.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://vxg.sxryk.cn

[R37] 把输出赋给变量
来源：http://siq.ctjpmb.com

files=$(ls -1)
来源：http://iad.jinqigfzy.top

[R38] 管道串联
来源：http://dwk.cdnleiting.top

cat a.txt | grep -i error | wc -l
来源：http://yyp.zhixingplan.top

[R39] 重定向标准输出与错误
来源：http://exh.ybcxt.top

cmd > out.log 2>&1
来源：http://xet.ydzc1.top

[R40] 追加写日志
来源：http://bnb.nanxuanxn.top

echo "log" >> out.log
来源：http://uva.gotoacloud.top

[R41] 丢弃输出
来源：http://nxr.cqqwz.cn

cmd >/dev/null 2>&1
来源：http://izy.fanxiaobao.xyz

[R42] 输入重定向
来源：http://wof.dashuyun.cn

wc -l < a.txt
来源：http://cep.jianghu66.top

[R43] 按名字查找文件
来源：http://ufh.zhiwuduotai.top

find . -name "*.log" -type f
来源：http://ayc.jqgufenzy.top

[R44] 按修改时间查找
来源：http://vux.tanke756.top

find . -mtime -7 -type f
来源：http://qzy.zhongyouzk.top

[R45] 批量删除
来源：http://ggs.quarkkingdee.top

find . -name "*.tmp" -delete
来源：http://zdt.nanxinkj.top

[R46] 递归替换文件内容
来源：http://nkv.epnwcf.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cra.yj20258888.top

[R47] sed 单行替换
来源：http://ueo.xuetiantiany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://afv.yuanzhike.top

[R48] awk 取指定列
来源：http://cek.jqgfzy.top

awk '{print $1, $3}' a.txt
来源：http://awq.yvedp.cn

[R49] awk 带条件
来源：http://ind.kuanghao11.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gls.316326.xyz

[R50] awk 求和
来源：http://oad.ivvv.top

awk '{s += $2} END {print s}' a.txt
来源：http://lxf.aibaodan.cn

[R51] 排序去重取前几
来源：http://zaw.tanke756.top

sort a.txt | uniq -c | sort -rn | head
来源：http://wyg.ppjwa.cn

[R52] 统计行数
来源：http://edw.ydjk.org.cn

wc -l a.txt
来源：http://jyj.hnxiangtu.top

[R53] 查看文件头与实时尾
来源：http://qop.cdnleiting.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://qcx.jinghuilouyu.cn

[R54] 比较两个文件
来源：http://ofy.ivvv.top

diff a.txt b.txt
来源：http://uci.jiagoushi.top

[R55] 压缩与解压
来源：http://fdn.fzhhl.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hfk.meibo888.top

[R56] 远程拷贝
来源：http://fib.yvedp.cn

scp file user@host:/path/
来源：http://rxk.svipenyu.cn

[R57] 远程执行命令
来源：http://ueo.meibo888.top

ssh user@host 'uptime'
来源：http://mup.nanxuanxn.top

[R58] 下载文件
来源：http://gpv.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qmg.shanyushiyangtech.top

[R59] 发 POST JSON
来源：http://rwu.yongpay.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rys.shanyushiyangkeji.top

[R60] 只看 HTTP 状态码
来源：http://mwu.nanxinkj.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ncz.9152youxi.cn

[R61] 磁盘占用
来源：http://wbv.zhongyouzk.top

df -h;  du -sh *
来源：http://khj.yj20258888.top

[R62] 找最占空间的文件
来源：http://vht.zhijiandao.cn

du -ah . | sort -rh | head -10
来源：http://rso.ivvv.top

[R63] 内存与进程
来源：http://iha.aibaodan.cn

free -h;  ps aux | grep nginx
来源：http://cix.snrcjt.cn

[R64] 结束进程
来源：http://ose.hysaishi.cn

kill -9 $(pgrep -f app.py)
来源：http://ujl.hcnkem.com

[R65] 查看端口占用
来源：http://oou.hongshengwenyu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://esf.iojbl.cn

[R66] 定时任务
来源：http://dyi.wangdashe.top

crontab -e;  crontab -l
来源：http://que.zhixingplan.top

[R67] 生成随机十六进制串
来源：http://bth.zhoulong.xyz

openssl rand -hex 16
来源：http://hqx.jinghuilouyu.cn

[R68] 计算文件校验值
来源：http://lah.ivvv.top

sha256sum a.txt;  md5sum a.txt
来源：http://pyq.sjlbkw.cn

[R69] 生成随机密码
来源：http://bul.daxiang520.top

head -c 16 /dev/urandom | base64
来源：http://pga.zhiwuduotai.top

[R70] 时间戳与互转
来源：http://tir.dianchejie.cn

date +%s;  date -d @1700000000
来源：http://aqh.iojbl.cn

[R71] 日期格式化
来源：http://zqc.jyoumei.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://blo.yueranfly.top

[R72] 等待端口就绪
来源：http://hyd.pengpengdd.cyou

until nc -z localhost 3306; do sleep 1; done
来源：http://pkb.0kj1m.cn

[R73] 分割大日志
来源：http://iho.wangshuangyany.cn

split -l 1000 big.log part_
来源：http://ezh.cucudq.cn

[R74] 批量重命名
来源：http://efq.fzhhl.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mge.yanxiufei.cn

[R75] 导出环境变量
来源：http://vdn.jianghu66.top

export PATH="$HOME/bin:$PATH"
来源：http://mtn.nanxuanxn.top

[R76] 使用临时文件
来源：http://jol.gzhubu.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wzt.hnqzz.top

[R77] 读取用户输入
来源：http://zyk.aizwys.cn

read -rp "请输入: " ans
来源：http://clf.yj20258888.top

[R78] 交互式菜单
来源：http://gou.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zxz.shanyushiyangtech.top

[R79] 解析命令行选项
来源：http://xbl.hysaishi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://epo.snrcjt.cn

[R80] 查看脚本执行耗时
来源：http://ofq.jianghu66.top

time ./run.sh
来源：http://fow.redwolf501.top

================================================================================
来源：http://pto.zdbjq.cn

S. C / C++ 专题
来源：http://iqx.iojbl.cn

================================================================================
来源：http://top.sweek.top

[S01] C：Hello World
来源：http://hls.xingfuxueyuan.xyz

#include <stdio.h>
来源：http://tfj.jyoumei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uvg.hesvh.cn

[S02] C：变量与格式化输出
来源：http://yyg.yj202588.top

int a = 10; printf("%d\n", a);
来源：http://ypl.9152youxi.cn

[S03] C：读入整数
来源：http://ezk.yvedp.cn

int x; scanf("%d", &x);
来源：http://yac.fktsv.cn

[S04] C：字符串复制
来源：http://wap.cheryme.top

char dst[32]; strcpy(dst, "hi");
来源：http://dzb.haohaochexian.top

[S05] C：字符串长度
来源：http://svx.daria6918.cn

strlen(s)
来源：http://ppt.cqqwz.cn

[S06] C：字符串比较
来源：http://gqk.dashuyun.cn

strcmp(a, b) == 0
来源：http://vck.zhixingplan.top

[S07] C：数组遍历求和
来源：http://raz.xziqi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sph.snrcjt.cn

[S08] C：动态内存分配与释放
来源：http://nss.shuidangran.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://urw.epnwcf.com

[S09] C：结构体定义与初始化
来源：http://ony.52xcode.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sln.yfazqb.com

[S10] C：指针与解引用
来源：http://tzi.pengpengdd.cyou

int *p = &a;  *p = 5;
来源：http://zru.sufxvd.cn

[S11] C：逐行读文件
来源：http://lod.vehdjk.com

FILE *f = fopen("a.txt", "r");
来源：http://rmb.haohaochexian.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://nwz.xinyue.icu

fclose(f);
来源：http://zdt.xuanzx.com

[S12] C：写文件
来源：http://imb.gotoacloud.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jgo.nanxinkj.top

[S13] C：宏定义
来源：http://vlx.52xcode.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aca.dashuyun.cn

[S14] C：枚举
来源：http://ztv.ehwqpu.com

enum Color { RED, GREEN, BLUE };
来源：http://bnz.cqqwz.cn

[S15] C：类型转换
来源：http://epg.zhoulong.xyz

(double) a / b
来源：http://kom.tianlin.xyz

[S16] C：位操作置位
来源：http://kkk.jinqigufen.top

x |= (1 << 3);
来源：http://kev.ybcxt.top

[S17] C：安全拼接字符串
来源：http://oso.cdnleiting.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wnp.tian-w.cn

[S18] C：命令行参数
来源：http://uns.nanxuanxn.top

int main(int argc, char **argv)
来源：http://bvg.daria6918.cn

[S19] C：快速排序
来源：http://vpw.jlsjyb.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hln.52xcode.cn

[S20] C：二分查找
来源：http://cfh.xuanzx.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://irz.ctjpmb.com

[S21] C：字符类别判断
来源：http://smp.feifeiyinyue.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://syr.uphjek.com

[S22] C：字符串转数字
来源：http://wiu.hcnkem.com

atoi("42");  strtod("3.14", NULL);
来源：http://whv.gotoacloud.top

[S23] C：随机数
来源：http://arv.vqdsnc.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ght.zhixingplan.top

[S24] C：获取本地时间
来源：http://saf.jqgufenzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gfj.svipenyu.cn

[S25] C：内存拷贝
来源：http://ceo.jianghu66.top

memcpy(dst, src, n);
来源：http://zzy.yangfankeji.com

[S26] C：内存清零
来源：http://fbe.jyoumei.cn

memset(a, 0, sizeof a);
来源：http://chj.jlsjyb.cn

[S27] C：定义常量
来源：http://ipd.sufxvd.cn

const double PI = 3.14159;
来源：http://daa.nwbrower.top

[S28] C：静态变量
来源：http://hxv.jqgufenzy.top

static int counter = 0;
来源：http://nkc.hnqzz.top

[S29] C：变参函数
来源：http://rkt.redwolf501.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rsx.jlsjyb.cn

[S30] C：头文件保护
来源：http://qze.chenjidiqi.icu

#ifndef X_H
来源：http://ykp.yuxming.cn

#define X_H
来源：http://xqh.zdbjq.cn

#endif
来源：http://kos.cashguo.top

[S31] C++：Hello World
来源：http://wsm.zhiwuduotai.top

#include <iostream>
来源：http://yka.jianghu66.top

int main() { std::cout << "Hello\n"; }
来源：http://crt.sysykeji.top

[S32] C++：字符串
来源：http://ixq.cdnleiting.top

std::string s = "hi";  s += "!";
来源：http://aec.wangdashe.top

[S33] C++：vector 增删
来源：http://kju.cashguo.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mpg.hesvh.cn

[S34] C++：遍历 vector
来源：http://hmc.jyoumei.cn

for (auto &x : v) { std::cout << x; }
来源：http://sqm.sufxvd.cn

[S35] C++：map
来源：http://zbx.xuetiantiany.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mgs.wangdashe.top

[S36] C++：unordered_map
来源：http://lmd.52xcode.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zsl.jinqigufen.top

[S37] C++：set
来源：http://nsd.jlsjyb.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://axj.zycfv.cn

[S38] C++：排序
来源：http://cim.sufxvd.cn

std::sort(v.begin(), v.end());
来源：http://cnq.fzhhl.top

[S39] C++：自定义比较器排序
来源：http://pzk.aibaodan.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zye.yfazqb.com

[S40] C++：查找元素
来源：http://lxt.hammf.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tvd.shzxlz.cn

[S41] C++：类与构造函数
来源：http://zkb.fehbvm.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qzc.yj202588.top

[S42] C++：继承与虚函数
来源：http://phe.ybcxt.top

class B : public Base { public: void f() override {} };
来源：http://emy.chenjidiqi.icu

[S43] C++：智能指针
来源：http://gqf.sweek.top

auto p = std::make_unique<int>(5);
来源：http://smc.jqgfzy.top

[S44] C++：引用传参
来源：http://xjx.cucudq.cn

void inc(int &x) { ++x; }
来源：http://jrl.cucudq.cn

[S45] C++：lambda
来源：http://nic.mhx1999.top

auto add = [](int a, int b) { return a + b; };
来源：http://oar.yuxming.cn

[S46] C++：函数模板
来源：http://col.tianlin.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vwz.aibaodan.cn

[S47] C++：结构化绑定遍历
来源：http://vdl.fengsongda.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ydz.hammf.cn

[S48] C++：逐行读文件
来源：http://rbu.yuxming.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pke.jqgfzy.top

while (std::getline(in, line)) { }
来源：http://heb.smart0.xyz

[S49] C++：写文件
来源：http://aad.hywenlv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://snj.hongshengwenyu.top

[S50] C++：格式化数字
来源：http://fcx.gotoacloud.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jvg.bjfxy.top

[S51] C++：显式类型转换
来源：http://kvl.cucudq.cn

static_cast<double>(a) / b
来源：http://pwo.zhaomingkeji.xyz

[S52] C++：const 与 noexcept
来源：http://pkl.hfpthk.cn

int size() const noexcept { return n_; }
来源：http://mgz.fktsv.cn

[S53] C++：移动语义
来源：http://npo.chenjidiqi.icu

std::vector<int> w = std::move(v);
来源：http://aeq.jinqigufen.top

[S54] C++：异常处理
来源：http://lno.zhengqikj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://acv.yvedp.cn

[S55] C++：结构化绑定
来源：http://jnc.jyoumei.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lgc.hesvh.cn

[S56] C++：optional
来源：http://pvz.hfpthk.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://aql.yonumen.top

[S57] C++：编译期常量
来源：http://btf.birdmap.top

constexpr int N = 10;
来源：http://jzk.feifeiyinyue.top

[S58] C++：命名空间
来源：http://hgn.wangdashe.top

namespace ns { int f() { return 1; } }
来源：http://rmu.yueranfly.top

[S59] C++：静态断言
来源：http://lin.yueranfly.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fyo.shuidangran.top

[S60] C++：遍历并删除元素
来源：http://rsp.jinqigufen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zzd.aibaodan.cn

================================================================================
来源：http://dlt.quarkkingdee.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qqr.bbcook.cn

================================================================================
来源：http://lzk.hnqzz.top

[T01] Kotlin：Hello World
来源：http://ajr.smart0.xyz

println("Hello")
来源：http://gox.zhiwuduotai.top

[T02] Kotlin：变量
来源：http://lld.gaohongyu789.top

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hhv.chenlongwang.top

[T03] Kotlin：字符串模板
来源：http://dtk.shzxlz.cn

"值: $b"
来源：http://gyn.cheryme.top

[T04] Kotlin：空安全
来源：http://vwq.guowangkeji.top

val n: String? = null;  n?.length
来源：http://itn.zhengqikj.top

[T05] Kotlin：when 表达式
来源：http://gbb.vehdjk.com

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jbe.ppjwa.cn

[T06] Kotlin：集合映射
来源：http://yhx.xuetiantiany.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ghb.uphjek.com

[T07] Kotlin：集合过滤
来源：http://gjg.cheryme.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://zjg.pengpengdd.cyou

[T08] Kotlin：数据类
来源：http://yav.aibaodan.cn

data class User(val name: String, val age: Int)
来源：http://ohk.birdmap.top

[T09] Kotlin：扩展函数
来源：http://vlg.yangfankeji.com

fun String.exclaim() = this + "!"
来源：http://pdp.hongshengwenyu.top

[T10] Kotlin：默认参数
来源：http://elr.shuidangran.top

fun greet(name: String = "World") = "Hi $name"
来源：http://zxx.chenjidiqi.icu

[T11] Kotlin：协程
来源：http://pln.vehdjk.com

GlobalScope.launch { delay(1000); println("done") }
来源：http://uoa.ctjpmb.com

[T12] Kotlin：解构声明
来源：http://jex.yanxiufei.cn

val (a, b) = Pair(1, 2)
来源：http://mqj.sysykeji.top

[T13] Kotlin：只读 Map
来源：http://tjf.feifeiyinyue.top

val m = mapOf("a" to 1)
来源：http://whv.daxiang520.top

[T14] Kotlin：循环
来源：http://zfh.vqdsnc.cn

for (i in 1..10) println(i)
来源：http://lou.yvedp.cn


<!-- 参考信息 -->