代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vci.smart0.xyz

[R10] 正则匹配
来源：http://tti.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bev.jinghuilouyu.cn

[R11] case 多分支
来源：http://kix.ydjk.org.cn

case "$1" in
来源：http://sgx.jinqigufen.top

start) echo "启动" ;;
来源：http://max.chenjidiqi.icu

stop)  echo "停止" ;;
来源：http://yth.ydzc1.top

*)     echo "未知命令" ;;
来源：http://ohd.0kj1m.cn

esac
来源：http://qre.jyoumei.cn

[R12] for 遍历文件
来源：http://fwj.iojbl.cn

for f in *.txt; do echo "$f"; done
来源：http://ziq.cqqwz.cn

[R13] for 计数循环
来源：http://kqd.shuidangran.top

for i in {1..10}; do echo "$i"; done
来源：http://ttq.fanxiaobao.xyz

[R14] C 风格 for
来源：http://lwh.nanxuanxn.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ceq.sjlbkw.cn

[R15] while 逐行读文件
来源：http://rrx.cheryme.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xyk.wangshuangyany.cn

[R16] until 等待条件
来源：http://lis.vehdjk.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gdp.fktsv.cn

[R17] 数组定义与取值
来源：http://zdf.yj20258.top

arr=(a b c); echo "${arr[0]}"
来源：http://nnp.xuanzx.com

[R18] 遍历数组
来源：http://lbi.nwbrower.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fea.sysykeji.top

[R19] 数组长度
来源：http://yrw.c1oappe.top

echo "${#arr[@]}"
来源：http://ygu.wangshuangyany.cn

[R20] 关联数组（字典）
来源：http://tqc.cheryme.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zdm.jinqigfzy.top

[R21] 字符串长度
来源：http://was.kuanghao11.cn

echo "${#s}"
来源：http://ljh.fengsongda.top

[R22] 截取子串
来源：http://rcu.zdbjq.cn

echo "${s:0:5}"
来源：http://nce.yanxiufei.cn

[R23] 字符串替换
来源：http://cyq.smart0.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://cnu.cqqwz.cn

[R24] 大小写转换
来源：http://wws.ctjpmb.com

echo "${s^^}"; echo "${s,,}"
来源：http://tqg.fzhhl.top

[R25] 去后缀 / 去前缀
来源：http://yzd.shanyushiyangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://cuo.sxryk.cn

[R26] 命令替换
来源：http://nnq.chenzaomai.com

now=$(date +%F); echo "$now"
来源：http://bty.ehwqpu.com

[R27] 算术展开
来源：http://yrj.ctjpmb.com

echo $((1 + 2 * 3))
来源：http://yhi.yuxming.cn

[R28] 浮点运算
来源：http://nri.yonumen.top

echo "scale=2; 10/3" | bc
来源：http://inc.redwolf501.top

[R29] 定义函数
来源：http://agf.sxryk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xxt.uphjek.com

[R30] 函数返回状态码
来源：http://ztf.zhixingplan.top

f() { return 0; }; f || echo "失败了"
来源：http://aob.ivvv.top

[R31] 局部变量
来源：http://gyc.cucudq.cn

f() { local x=1; echo "$x"; }
来源：http://lva.yj20258.top

[R32] 参数个数校验
来源：http://aem.wangdashe.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ztj.ydzc1.top

[R33] 捕获错误并提示行号
来源：http://cge.ydzc1.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jsy.pycfn.com

[R34] 退出时清理
来源：http://mzv.mhx1999.top

trap 'rm -f "$tmp"' EXIT
来源：http://tcc.gzhubu.top

[R35] 后台执行并等待
来源：http://fyg.tarul.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jaj.tarul.cn

[R36] 并发执行多个任务
来源：http://dvg.epnwcf.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://gkh.hongshengwenyu.top

[R37] 把输出赋给变量
来源：http://ouv.c1oappe.top

files=$(ls -1)
来源：http://ima.hnxiangtu.top

[R38] 管道串联
来源：http://eua.pengpengdd.cyou

cat a.txt | grep -i error | wc -l
来源：http://ldp.zdbjq.cn

[R39] 重定向标准输出与错误
来源：http://ovj.aizwys.cn

cmd > out.log 2>&1
来源：http://mjh.daxiang520.top

[R40] 追加写日志
来源：http://jrt.yuanzhike.top

echo "log" >> out.log
来源：http://zwc.kuanghao11.cn

[R41] 丢弃输出
来源：http://xgl.daria6918.cn

cmd >/dev/null 2>&1
来源：http://qfz.hesvh.cn

[R42] 输入重定向
来源：http://xej.c1oappe.top

wc -l < a.txt
来源：http://fqn.tarul.cn

[R43] 按名字查找文件
来源：http://bra.yanxiufei.cn

find . -name "*.log" -type f
来源：http://bik.zhongyouzk.top

[R44] 按修改时间查找
来源：http://wvu.sxryk.cn

find . -mtime -7 -type f
来源：http://xto.feifeiyinyue.top

[R45] 批量删除
来源：http://pwe.xylfe.cn

find . -name "*.tmp" -delete
来源：http://idg.gzhubu.top

[R46] 递归替换文件内容
来源：http://gkn.fengsongda.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://euv.hcnkem.com

[R47] sed 单行替换
来源：http://cwq.yonumen.top

sed -i 's/foo/bar/g' a.txt
来源：http://lwc.kuanghao11.cn

[R48] awk 取指定列
来源：http://qvg.smart0.xyz

awk '{print $1, $3}' a.txt
来源：http://vcz.sysykeji.top

[R49] awk 带条件
来源：http://njo.jqgufenzy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cvn.gogol.net.cn

[R50] awk 求和
来源：http://vez.zhiwuduotai.top

awk '{s += $2} END {print s}' a.txt
来源：http://gxr.vehdjk.com

[R51] 排序去重取前几
来源：http://lra.meibo888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://efb.cheryme.top

[R52] 统计行数
来源：http://ytw.uphjek.com

wc -l a.txt
来源：http://tju.cdnleiting.top

[R53] 查看文件头与实时尾
来源：http://wix.andypj.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zmu.feifeiyinyue.top

[R54] 比较两个文件
来源：http://wic.zycfv.cn

diff a.txt b.txt
来源：http://ztt.meibo888.top

[R55] 压缩与解压
来源：http://ftr.zycfv.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hut.yvedp.cn

[R56] 远程拷贝
来源：http://gha.ehwqpu.com

scp file user@host:/path/
来源：http://xbr.zhixingplan.top

[R57] 远程执行命令
来源：http://dxv.havefunace.top

ssh user@host 'uptime'
来源：http://pen.gogol.net.cn

[R58] 下载文件
来源：http://drl.jianghu66.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://foo.shuidangran.top

[R59] 发 POST JSON
来源：http://kjx.havefunace.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://iyo.ppjwa.cn

[R60] 只看 HTTP 状态码
来源：http://prg.redwolf501.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rqm.nanxuanxn.top

[R61] 磁盘占用
来源：http://vvc.shuidangran.top

df -h;  du -sh *
来源：http://sla.cheryme.top

[R62] 找最占空间的文件
来源：http://agg.iojbl.cn

du -ah . | sort -rh | head -10
来源：http://vzq.chenlongwang.top

[R63] 内存与进程
来源：http://wrh.nwbrower.top

free -h;  ps aux | grep nginx
来源：http://dda.cashguo.top

[R64] 结束进程
来源：http://yqs.wangshuangyany.cn

kill -9 $(pgrep -f app.py)
来源：http://wmv.feifeiyinyue.top

[R65] 查看端口占用
来源：http://ujy.xylfe.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ytq.haohaochexian.top

[R66] 定时任务
来源：http://ewx.wangshuangyany.cn

crontab -e;  crontab -l
来源：http://rze.zdbjq.cn

[R67] 生成随机十六进制串
来源：http://sbi.hammf.cn

openssl rand -hex 16
来源：http://ocu.yanxiufei.cn

[R68] 计算文件校验值
来源：http://vgx.zhoulong.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://sbi.chenjidiqi.icu

[R69] 生成随机密码
来源：http://okg.zhoulong.xyz

head -c 16 /dev/urandom | base64
来源：http://cgt.chenjidiqi.icu

[R70] 时间戳与互转
来源：http://gnn.epnwcf.com

date +%s;  date -d @1700000000
来源：http://zup.zhoulong.xyz

[R71] 日期格式化
来源：http://ecm.chenjidiqi.icu

date +"%Y-%m-%d %H:%M:%S"
来源：http://sfs.gogol.net.cn

[R72] 等待端口就绪
来源：http://yno.bjfxy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://yxx.andypj.xyz

[R73] 分割大日志
来源：http://mem.wangshuangyany.cn

split -l 1000 big.log part_
来源：http://hnn.zhixingplan.top

[R74] 批量重命名
来源：http://dor.yueranfly.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://akf.zdbjq.cn

[R75] 导出环境变量
来源：http://dds.9152youxi.cn

export PATH="$HOME/bin:$PATH"
来源：http://qxu.dashuyun.cn

[R76] 使用临时文件
来源：http://njp.quarkkingdee.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://geu.jyoumei.cn

[R77] 读取用户输入
来源：http://rvt.yj202588.top

read -rp "请输入: " ans
来源：http://gpn.shanyushiyangkeji.top

[R78] 交互式菜单
来源：http://ful.chenjidiqi.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://qrt.xingfuxueyuan.xyz

[R79] 解析命令行选项
来源：http://fst.ctjpmb.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ojx.fzhhl.top

[R80] 查看脚本执行耗时
来源：http://zmv.epnwcf.com

time ./run.sh
来源：http://cbc.gotoacloud.top

================================================================================
来源：http://xmb.ehwqpu.com

S. C / C++ 专题
来源：http://kqk.9152youxi.cn

================================================================================
来源：http://hqb.tianlin.xyz

[S01] C：Hello World
来源：http://wnm.pengpengdd.cyou

#include <stdio.h>
来源：http://qnl.zhengqikj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://byv.fanxiaobao.xyz

[S02] C：变量与格式化输出
来源：http://umg.jinqigufen.top

int a = 10; printf("%d\n", a);
来源：http://ajr.zycfv.cn

[S03] C：读入整数
来源：http://emx.guannengcc.top

int x; scanf("%d", &x);
来源：http://kgr.zhoulong.xyz

[S04] C：字符串复制
来源：http://bec.yongpay.top

char dst[32]; strcpy(dst, "hi");
来源：http://kac.jlsjyb.cn

[S05] C：字符串长度
来源：http://oyo.xuanzx.com

strlen(s)
来源：http://cqx.svipenyu.cn

[S06] C：字符串比较
来源：http://udn.svipenyu.cn

strcmp(a, b) == 0
来源：http://evs.52xcode.cn

[S07] C：数组遍历求和
来源：http://ucy.jinqigufen.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://udc.hfpthk.cn

[S08] C：动态内存分配与释放
来源：http://vwu.smart0.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mfc.cucudq.cn

[S09] C：结构体定义与初始化
来源：http://elr.guowangkeji.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ulu.yj20258888.top

[S10] C：指针与解引用
来源：http://rym.zycfv.cn

int *p = &a;  *p = 5;
来源：http://qgk.zhoulong.xyz

[S11] C：逐行读文件
来源：http://zlx.hysaishi.cn

FILE *f = fopen("a.txt", "r");
来源：http://szf.jlsjyb.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lfz.zhongyouzk.top

fclose(f);
来源：http://obf.jlsjyb.cn

[S12] C：写文件
来源：http://rgi.nanxuanxn.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kcu.yuxming.cn

[S13] C：宏定义
来源：http://spy.vqdsnc.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://txp.yj20258.top

[S14] C：枚举
来源：http://lcy.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://ljz.zhijiandao.cn

[S15] C：类型转换
来源：http://wqo.chenjidiqi.icu

(double) a / b
来源：http://pfo.yj202588.top

[S16] C：位操作置位
来源：http://whp.hesvh.cn

x |= (1 << 3);
来源：http://aly.kuanghao11.cn

[S17] C：安全拼接字符串
来源：http://oan.gogol.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://van.hcnkem.com

[S18] C：命令行参数
来源：http://hyv.chenzaomai.com

int main(int argc, char **argv)
来源：http://frs.xuanzx.com

[S19] C：快速排序
来源：http://mek.meibo888.top

qsort(a, n, sizeof(int), cmp);
来源：http://rgq.hnqzz.top

[S20] C：二分查找
来源：http://ooj.jinqigfzy.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qbl.shanyushiyangtech.top

[S21] C：字符类别判断
来源：http://vqv.hfpthk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bvp.chenjidiqi.icu

[S22] C：字符串转数字
来源：http://ryj.zhixingplan.top

atoi("42");  strtod("3.14", NULL);
来源：http://qnd.xingfuxueyuan.xyz

[S23] C：随机数
来源：http://hhq.zhongyouzk.top

srand(time(NULL));  int r = rand() % 100;
来源：http://lag.xylfe.cn

[S24] C：获取本地时间
来源：http://eva.xingfuxueyuan.xyz

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kzx.svipenyu.cn

[S25] C：内存拷贝
来源：http://hzx.jinghuilouyu.cn

memcpy(dst, src, n);
来源：http://zuo.daria6918.cn

[S26] C：内存清零
来源：http://ysx.shanyushiyangtech.top

memset(a, 0, sizeof a);
来源：http://tvq.hysaishi.cn

[S27] C：定义常量
来源：http://idj.hnxiangtu.top

const double PI = 3.14159;
来源：http://tzt.fktsv.cn

[S28] C：静态变量
来源：http://mzj.fehbvm.com

static int counter = 0;
来源：http://nxz.pycfn.com

[S29] C：变参函数
来源：http://vqd.jqgufenzy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://aqi.chenlongwang.top

[S30] C：头文件保护
来源：http://cmh.vehdjk.com

#ifndef X_H
来源：http://ttj.snrcjt.cn

#define X_H
来源：http://qnk.pengpengdd.cyou

#endif
来源：http://ldg.xuetiantiany.cn

[S31] C++：Hello World
来源：http://ema.uphjek.com

#include <iostream>
来源：http://ewj.quarkkingdee.top

int main() { std::cout << "Hello\n"; }
来源：http://gyo.c1oappe.top

[S32] C++：字符串
来源：http://fdi.fehbvm.com

std::string s = "hi";  s += "!";
来源：http://slx.jinqigfzy.top

[S33] C++：vector 增删
来源：http://qjo.mhx1999.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zty.jinqigufen.top

[S34] C++：遍历 vector
来源：http://lrr.yonumen.top

for (auto &x : v) { std::cout << x; }
来源：http://dqh.zycfv.cn

[S35] C++：map
来源：http://bpg.zdbjq.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qze.ybcxt.top

[S36] C++：unordered_map
来源：http://ibn.pengpengdd.cyou

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jxk.havefunace.top

[S37] C++：set
来源：http://nge.yj20258888.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bpu.yueranfly.top

[S38] C++：排序
来源：http://ehq.fzhhl.top

std::sort(v.begin(), v.end());
来源：http://ivd.zhiwuduotai.top

[S39] C++：自定义比较器排序
来源：http://saf.hnqzz.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://htd.sweek.top

[S40] C++：查找元素
来源：http://chw.shanyushiyangkeji.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zmd.wangshuangyany.cn

[S41] C++：类与构造函数
来源：http://tqo.aizwys.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ezw.birdmap.top

[S42] C++：继承与虚函数
来源：http://rfi.yonumen.top

class B : public Base { public: void f() override {} };
来源：http://cqe.wangshuangyany.cn

[S43] C++：智能指针
来源：http://uzu.hnqzz.top

auto p = std::make_unique<int>(5);
来源：http://dnl.yangfankeji.com

[S44] C++：引用传参
来源：http://kak.xuanzx.com

void inc(int &x) { ++x; }
来源：http://rid.shzxlz.cn

[S45] C++：lambda
来源：http://gwt.quarkkingdee.top

auto add = [](int a, int b) { return a + b; };
来源：http://hgz.gogol.net.cn

[S46] C++：函数模板
来源：http://tei.ehwqpu.com

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://rbg.guannengcc.top

[S47] C++：结构化绑定遍历
来源：http://hmy.zhixingplan.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vlp.hysaishi.cn

[S48] C++：逐行读文件
来源：http://qja.yj202588.top

std::ifstream in("a.txt");  std::string line;
来源：http://ans.316326.xyz

while (std::getline(in, line)) { }
来源：http://bes.ywan-chungtsiang.top

[S49] C++：写文件
来源：http://wnp.gotoacloud.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uoj.yuxming.cn

[S50] C++：格式化数字
来源：http://yhx.hcnkem.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zhg.sysykeji.top

[S51] C++：显式类型转换
来源：http://hyz.sufxvd.cn

static_cast<double>(a) / b
来源：http://kxy.hfpthk.cn

[S52] C++：const 与 noexcept
来源：http://eyr.zdbjq.cn

int size() const noexcept { return n_; }
来源：http://yfj.hongshengwenyu.top

[S53] C++：移动语义
来源：http://vit.aizwys.cn

std::vector<int> w = std::move(v);
来源：http://slb.ehwqpu.com

[S54] C++：异常处理
来源：http://yhx.cqqwz.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://pdt.tian-w.cn

[S55] C++：结构化绑定
来源：http://nrw.bjfxy.top

auto [a, b] = std::make_pair(1, 2);
来源：http://une.meibo888.top

[S56] C++：optional
来源：http://pvx.nanxinkj.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://fga.vehdjk.com

[S57] C++：编译期常量
来源：http://bhy.yuxming.cn

constexpr int N = 10;
来源：http://baw.epnwcf.com

[S58] C++：命名空间
来源：http://fdf.xuetiantiany.cn

namespace ns { int f() { return 1; } }
来源：http://ygs.bjfxy.top

[S59] C++：静态断言
来源：http://nog.gotoacloud.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tcu.zhengqikj.top

[S60] C++：遍历并删除元素
来源：http://bbb.shanyushiyangkeji.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jyl.hesvh.cn

================================================================================
来源：http://npd.guowangkeji.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ciu.epnwcf.com

================================================================================
来源：http://spu.yanxiufei.cn

[T01] Kotlin：Hello World
来源：http://rpl.ivvv.top

println("Hello")
来源：http://ciq.ctjpmb.com

[T02] Kotlin：变量
来源：http://vpv.sjlbkw.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vop.sysykeji.top

[T03] Kotlin：字符串模板
来源：http://vfc.jinqigufen.top

"值: $b"
来源：http://maw.fanxiaobao.xyz

[T04] Kotlin：空安全
来源：http://jua.guowangkeji.top

val n: String? = null;  n?.length
来源：http://ygi.yangfankeji.com

[T05] Kotlin：when 表达式
来源：http://bya.316326.xyz

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gmo.jyoumei.cn

[T06] Kotlin：集合映射
来源：http://wxc.yj20258888.top

listOf(1, 2, 3).map { it * 2 }
来源：http://ehj.xingfuxueyuan.xyz

[T07] Kotlin：集合过滤
来源：http://mdx.yuanzhike.top

listOf(1, 2, 3).filter { it > 1 }
来源：http://ala.jinqigfzy.top

[T08] Kotlin：数据类
来源：http://wxv.shangyingyoupin.top

data class User(val name: String, val age: Int)
来源：http://sjo.yfazqb.com

[T09] Kotlin：扩展函数
来源：http://qad.redwolf501.top

fun String.exclaim() = this + "!"
来源：http://suz.hammf.cn

[T10] Kotlin：默认参数
来源：http://nha.sysykeji.top

fun greet(name: String = "World") = "Hi $name"
来源：http://vhu.svipenyu.cn


<!-- 参考信息 -->