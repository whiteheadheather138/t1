代发 wailian999

R. Bash 专题
来源：http://nrc.daria6918.cn

================================================================================
来源：http://yxq.jinyuanbaomall.cn

[R01] shebang 与严格模式
来源：http://had.hnxiangtu.top

#!/usr/bin/env bash
来源：http://fly.xziqi.cn

set -euo pipefail
来源：http://dds.cdnleiting.top

[R02] 变量赋值与使用
来源：http://okt.pycfn.com

name="Tom"; echo "$name"
来源：http://wpk.shangyingyoupin.top

[R03] 只读变量
来源：http://pbh.sufxvd.cn

readonly PI=3.14
来源：http://icf.xingfuxueyuan.xyz

[R04] 位置参数
来源：http://swm.yuanzhike.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://xqq.zhoulong.xyz

[R05] 参数默认值
来源：http://fjw.sweek.top

name="${1:-default}"
来源：http://qfd.hnxiangtu.top

[R06] 判断命令是否存在
来源：http://hba.fanxiaobao.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ops.jqgfzy.top

[R07] if 判断文件
来源：http://cbl.kuanghao11.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://fta.ppjwa.cn

[R08] 数值比较
来源：http://emj.guowangkeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://yyj.ppjwa.cn

[R09] 字符串比较
来源：http://lwr.nanxuanxn.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://tkp.xuanzx.com

[R10] 正则匹配
来源：http://ket.quarkkingdee.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tla.chenlongwang.top

[R11] case 多分支
来源：http://vdh.zdqjudy.top

case "$1" in
来源：http://wqf.ivvv.top

start) echo "启动" ;;
来源：http://zel.9152youxi.cn

stop)  echo "停止" ;;
来源：http://vuu.xingfuxueyuan.xyz

*)     echo "未知命令" ;;
来源：http://dzo.jinqigufen.top

esac
来源：http://nqf.jinyuanbaomall.cn

[R12] for 遍历文件
来源：http://nah.tarul.cn

for f in *.txt; do echo "$f"; done
来源：http://rfe.hammf.cn

[R13] for 计数循环
来源：http://oxu.jinqigufen.top

for i in {1..10}; do echo "$i"; done
来源：http://imc.cqqwz.cn

[R14] C 风格 for
来源：http://yok.shuidangran.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iny.xylfe.cn

[R15] while 逐行读文件
来源：http://khl.jyoumei.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tml.gaohongyu789.top

[R16] until 等待条件
来源：http://wab.zycfv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qyr.ydzc1.top

[R17] 数组定义与取值
来源：http://mrw.bbcook.cn

arr=(a b c); echo "${arr[0]}"
来源：http://rez.ehwqpu.com

[R18] 遍历数组
来源：http://wdi.hnqzz.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cfj.hongshengwenyu.top

[R19] 数组长度
来源：http://rbc.bjfxy.top

echo "${#arr[@]}"
来源：http://piz.zhiwuduotai.top

[R20] 关联数组（字典）
来源：http://kbj.pycfn.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lom.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://qgc.zdqjudy.top

echo "${#s}"
来源：http://jkn.feifeiyinyue.top

[R22] 截取子串
来源：http://qsr.jiagoushi.top

echo "${s:0:5}"
来源：http://cbv.xylfe.cn

[R23] 字符串替换
来源：http://ugl.xuanzx.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://pzx.tian-w.cn

[R24] 大小写转换
来源：http://vdd.epnwcf.com

echo "${s^^}"; echo "${s,,}"
来源：http://lta.gaohongyu789.top

[R25] 去后缀 / 去前缀
来源：http://dhs.zhongyouzk.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ccf.xingfuxueyuan.xyz

[R26] 命令替换
来源：http://tit.9152youxi.cn

now=$(date +%F); echo "$now"
来源：http://cml.ctjpmb.com

[R27] 算术展开
来源：http://usv.sysykeji.top

echo $((1 + 2 * 3))
来源：http://tqy.sysykeji.top

[R28] 浮点运算
来源：http://qrh.hywenlv.cn

echo "scale=2; 10/3" | bc
来源：http://foz.yangfankeji.com

[R29] 定义函数
来源：http://sxx.shuidangran.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kwk.sufxvd.cn

[R30] 函数返回状态码
来源：http://gkw.cucudq.cn

f() { return 0; }; f || echo "失败了"
来源：http://bzc.gzhubu.top

[R31] 局部变量
来源：http://igc.fanxiaobao.xyz

f() { local x=1; echo "$x"; }
来源：http://man.birdmap.top

[R32] 参数个数校验
来源：http://mya.yfazqb.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ghc.zhengqikj.top

[R33] 捕获错误并提示行号
来源：http://ukl.chenlongwang.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://itt.tarul.cn

[R34] 退出时清理
来源：http://kxb.zhiwuduotai.top

trap 'rm -f "$tmp"' EXIT
来源：http://laz.zhoulong.xyz

[R35] 后台执行并等待
来源：http://hyg.hysaishi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fhg.zycfv.cn

[R36] 并发执行多个任务
来源：http://pfg.daria6918.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://odw.yj202588.top

[R37] 把输出赋给变量
来源：http://xwe.sufxvd.cn

files=$(ls -1)
来源：http://fff.hnqzz.top

[R38] 管道串联
来源：http://dqt.hywenlv.cn

cat a.txt | grep -i error | wc -l
来源：http://hnp.jlsjyb.cn

[R39] 重定向标准输出与错误
来源：http://ufn.fktsv.cn

cmd > out.log 2>&1
来源：http://sgf.tarul.cn

[R40] 追加写日志
来源：http://prx.yj20258888.top

echo "log" >> out.log
来源：http://rpw.ivvv.top

[R41] 丢弃输出
来源：http://oja.yuanzhike.top

cmd >/dev/null 2>&1
来源：http://eyy.nanxinkj.top

[R42] 输入重定向
来源：http://ngg.tianlin.xyz

wc -l < a.txt
来源：http://mss.yanxiufei.cn

[R43] 按名字查找文件
来源：http://mlp.birdmap.top

find . -name "*.log" -type f
来源：http://upl.epnwcf.com

[R44] 按修改时间查找
来源：http://ryi.hammf.cn

find . -mtime -7 -type f
来源：http://nva.hesvh.cn

[R45] 批量删除
来源：http://aim.iojbl.cn

find . -name "*.tmp" -delete
来源：http://tjn.cqqwz.cn

[R46] 递归替换文件内容
来源：http://fhs.zhoulong.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vse.xuanzx.com

[R47] sed 单行替换
来源：http://qyu.birdmap.top

sed -i 's/foo/bar/g' a.txt
来源：http://sqv.jinghuilouyu.cn

[R48] awk 取指定列
来源：http://pwd.xziqi.cn

awk '{print $1, $3}' a.txt
来源：http://wyv.jinqigfzy.top

[R49] awk 带条件
来源：http://bep.xingfuxueyuan.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://otr.ppjwa.cn

[R50] awk 求和
来源：http://evb.yueranfly.top

awk '{s += $2} END {print s}' a.txt
来源：http://gxz.vqdsnc.cn

[R51] 排序去重取前几
来源：http://wje.chenzaomai.com

sort a.txt | uniq -c | sort -rn | head
来源：http://ufk.zhongyouzk.top

[R52] 统计行数
来源：http://azi.yangfankeji.com

wc -l a.txt
来源：http://ali.ywan-chungtsiang.top

[R53] 查看文件头与实时尾
来源：http://xoz.ivvv.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bgk.jinqigfzy.top

[R54] 比较两个文件
来源：http://mhz.xinyue.icu

diff a.txt b.txt
来源：http://lia.zdqjudy.top

[R55] 压缩与解压
来源：http://xhg.smart0.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hwu.jlsjyb.cn

[R56] 远程拷贝
来源：http://ewq.bbcook.cn

scp file user@host:/path/
来源：http://tei.aizwys.cn

[R57] 远程执行命令
来源：http://pso.ydjk.org.cn

ssh user@host 'uptime'
来源：http://sef.zhoulong.xyz

[R58] 下载文件
来源：http://yzv.zhijiandao.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jrx.ppjwa.cn

[R59] 发 POST JSON
来源：http://aee.fanxiaobao.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tcx.dashuyun.cn

[R60] 只看 HTTP 状态码
来源：http://rev.jianghu66.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gel.vehdjk.com

[R61] 磁盘占用
来源：http://rgh.hnxiangtu.top

df -h;  du -sh *
来源：http://ewf.fktsv.cn

[R62] 找最占空间的文件
来源：http://agv.kuanghao11.cn

du -ah . | sort -rh | head -10
来源：http://eyd.guannengcc.top

[R63] 内存与进程
来源：http://lyv.xylfe.cn

free -h;  ps aux | grep nginx
来源：http://bjl.shuidangran.top

[R64] 结束进程
来源：http://pjv.fehbvm.com

kill -9 $(pgrep -f app.py)
来源：http://wtc.sufxvd.cn

[R65] 查看端口占用
来源：http://osj.jqgufenzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bcp.meibo888.top

[R66] 定时任务
来源：http://fpc.xinyue.icu

crontab -e;  crontab -l
来源：http://pjy.zdbjq.cn

[R67] 生成随机十六进制串
来源：http://wiv.yvedp.cn

openssl rand -hex 16
来源：http://hmw.gaohongyu789.top

[R68] 计算文件校验值
来源：http://nns.sxryk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uuh.dianchejie.cn

[R69] 生成随机密码
来源：http://nbr.ybcxt.top

head -c 16 /dev/urandom | base64
来源：http://iig.fehbvm.com

[R70] 时间戳与互转
来源：http://qtp.jyoumei.cn

date +%s;  date -d @1700000000
来源：http://kji.smart0.xyz

[R71] 日期格式化
来源：http://vck.yfazqb.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://ojj.shzxlz.cn

[R72] 等待端口就绪
来源：http://iez.gaohongyu789.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zxe.cheryme.top

[R73] 分割大日志
来源：http://qqf.chenlongwang.top

split -l 1000 big.log part_
来源：http://yhw.yonumen.top

[R74] 批量重命名
来源：http://jfq.zhixingplan.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vdv.bjfxy.top

[R75] 导出环境变量
来源：http://twe.ppjwa.cn

export PATH="$HOME/bin:$PATH"
来源：http://hws.zycfv.cn

[R76] 使用临时文件
来源：http://hju.mhx1999.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zcw.cqqwz.cn

[R77] 读取用户输入
来源：http://xjr.tanke756.top

read -rp "请输入: " ans
来源：http://caz.guowangkeji.top

[R78] 交互式菜单
来源：http://umr.sweek.top

select opt in a b c; do echo "$opt"; break; done
来源：http://dxi.jinqigufen.top

[R79] 解析命令行选项
来源：http://jfk.andypj.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qzf.yangfankeji.com

[R80] 查看脚本执行耗时
来源：http://rfd.tianlin.xyz

time ./run.sh
来源：http://lyh.jlsjyb.cn

================================================================================
来源：http://anj.ppjwa.cn

S. C / C++ 专题
来源：http://rvq.tianlin.xyz

================================================================================
来源：http://rzt.zycfv.cn

[S01] C：Hello World
来源：http://bqe.xingfuxueyuan.xyz

#include <stdio.h>
来源：http://kjk.zhijiandao.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jor.9152youxi.cn

[S02] C：变量与格式化输出
来源：http://wyo.yuxming.cn

int a = 10; printf("%d\n", a);
来源：http://dwz.fktsv.cn

[S03] C：读入整数
来源：http://lck.0kj1m.cn

int x; scanf("%d", &x);
来源：http://whk.fengsongda.top

[S04] C：字符串复制
来源：http://fdb.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mcl.yonumen.top

[S05] C：字符串长度
来源：http://bzo.sweek.top

strlen(s)
来源：http://pau.jinqigufen.top

[S06] C：字符串比较
来源：http://mhy.sjlbkw.cn

strcmp(a, b) == 0
来源：http://fmx.epnwcf.com

[S07] C：数组遍历求和
来源：http://vts.smart0.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://obb.cucudq.cn

[S08] C：动态内存分配与释放
来源：http://dzb.wangshuangyany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cdk.snrcjt.cn

[S09] C：结构体定义与初始化
来源：http://beq.gzhubu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nrz.kuanghao11.cn

[S10] C：指针与解引用
来源：http://qft.birdmap.top

int *p = &a;  *p = 5;
来源：http://uhw.zhengqikj.top

[S11] C：逐行读文件
来源：http://mea.yuanzhike.top

FILE *f = fopen("a.txt", "r");
来源：http://wvv.zhiwuduotai.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dyg.yongpay.top

fclose(f);
来源：http://naw.ydzc1.top

[S12] C：写文件
来源：http://pkd.meibo888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://uff.zycfv.cn

[S13] C：宏定义
来源：http://jso.nanxinkj.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uhk.gaohongyu789.top

[S14] C：枚举
来源：http://wjq.jiagoushi.top

enum Color { RED, GREEN, BLUE };
来源：http://mrx.zhixingplan.top

[S15] C：类型转换
来源：http://bxf.316326.xyz

(double) a / b
来源：http://ueq.jqgfzy.top

[S16] C：位操作置位
来源：http://qzr.wangdashe.top

x |= (1 << 3);
来源：http://zsg.tianlin.xyz

[S17] C：安全拼接字符串
来源：http://mzp.sweek.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tau.nanxuanxn.top

[S18] C：命令行参数
来源：http://upn.tarul.cn

int main(int argc, char **argv)
来源：http://owo.guannengcc.top

[S19] C：快速排序
来源：http://lrj.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ghg.fehbvm.com

[S20] C：二分查找
来源：http://bdy.yanxiufei.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lsm.xziqi.cn

[S21] C：字符类别判断
来源：http://qvi.hysaishi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jgi.zhoulong.xyz

[S22] C：字符串转数字
来源：http://vyo.jinyuanbaomall.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ibn.ivvv.top

[S23] C：随机数
来源：http://rgv.yj20258888.top

srand(time(NULL));  int r = rand() % 100;
来源：http://uts.yongpay.top

[S24] C：获取本地时间
来源：http://vga.epnwcf.com

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://owe.shanyushiyangkeji.top

[S25] C：内存拷贝
来源：http://ljm.haohaochexian.top

memcpy(dst, src, n);
来源：http://qhv.yuanzhike.top

[S26] C：内存清零
来源：http://jmt.zhijiandao.cn

memset(a, 0, sizeof a);
来源：http://mbu.hnxiangtu.top

[S27] C：定义常量
来源：http://rva.jinqigfzy.top

const double PI = 3.14159;
来源：http://ych.dianchejie.cn

[S28] C：静态变量
来源：http://qvs.hnqzz.top

static int counter = 0;
来源：http://ior.ehwqpu.com

[S29] C：变参函数
来源：http://vcz.yonumen.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://crw.feifeiyinyue.top

[S30] C：头文件保护
来源：http://ugu.hammf.cn

#ifndef X_H
来源：http://rzh.pengpengdd.cyou

#define X_H
来源：http://drz.fanxiaobao.xyz

#endif
来源：http://nbc.nanxinkj.top

[S31] C++：Hello World
来源：http://mnm.hongshengwenyu.top

#include <iostream>
来源：http://ele.chenlongwang.top

int main() { std::cout << "Hello\n"; }
来源：http://pcn.0kj1m.cn

[S32] C++：字符串
来源：http://gqs.daria6918.cn

std::string s = "hi";  s += "!";
来源：http://hto.c1oappe.top

[S33] C++：vector 增删
来源：http://hij.dashuyun.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gyc.gogol.net.cn

[S34] C++：遍历 vector
来源：http://eib.hesvh.cn

for (auto &x : v) { std::cout << x; }
来源：http://ycp.zhaomingkeji.xyz

[S35] C++：map
来源：http://yiz.zycfv.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qzz.yonumen.top

[S36] C++：unordered_map
来源：http://wrp.gaohongyu789.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://atu.zycfv.cn

[S37] C++：set
来源：http://lvb.sufxvd.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://chi.ehwqpu.com

[S38] C++：排序
来源：http://ntn.zhiwuduotai.top

std::sort(v.begin(), v.end());
来源：http://tsk.vqdsnc.cn

[S39] C++：自定义比较器排序
来源：http://iyz.uphjek.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gix.yvedp.cn

[S40] C++：查找元素
来源：http://eya.fehbvm.com

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kjs.tarul.cn

[S41] C++：类与构造函数
来源：http://vow.vehdjk.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xrd.ybcxt.top

[S42] C++：继承与虚函数
来源：http://mqh.cucudq.cn

class B : public Base { public: void f() override {} };
来源：http://ied.fehbvm.com

[S43] C++：智能指针
来源：http://mtu.uphjek.com

auto p = std::make_unique<int>(5);
来源：http://dle.ppjwa.cn

[S44] C++：引用传参
来源：http://ljp.yanxiufei.cn

void inc(int &x) { ++x; }
来源：http://ovf.sufxvd.cn

[S45] C++：lambda
来源：http://omv.pycfn.com

auto add = [](int a, int b) { return a + b; };
来源：http://kog.52xcode.cn

[S46] C++：函数模板
来源：http://kxa.yuanzhike.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jdf.9152youxi.cn

[S47] C++：结构化绑定遍历
来源：http://ods.smart0.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://exf.cucudq.cn

[S48] C++：逐行读文件
来源：http://guu.sweek.top

std::ifstream in("a.txt");  std::string line;
来源：http://bgl.jianghu66.top

while (std::getline(in, line)) { }
来源：http://zmk.yangfankeji.com

[S49] C++：写文件
来源：http://tyb.yonumen.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gcr.sysykeji.top

[S50] C++：格式化数字
来源：http://lxy.c1oappe.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lvb.sxryk.cn

[S51] C++：显式类型转换
来源：http://dei.jlsjyb.cn

static_cast<double>(a) / b
来源：http://qpl.cqqwz.cn

[S52] C++：const 与 noexcept
来源：http://tdp.tian-w.cn

int size() const noexcept { return n_; }
来源：http://itg.zhoulong.xyz

[S53] C++：移动语义
来源：http://ltf.zhiwuduotai.top

std::vector<int> w = std::move(v);
来源：http://tad.hongshengwenyu.top

[S54] C++：异常处理
来源：http://wpz.zycfv.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qnf.hfpthk.cn

[S55] C++：结构化绑定
来源：http://hcz.tian-w.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pig.snrcjt.cn

[S56] C++：optional
来源：http://sxk.fanxiaobao.xyz

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://foo.jyoumei.cn

[S57] C++：编译期常量
来源：http://mre.fanxiaobao.xyz

constexpr int N = 10;
来源：http://weq.vehdjk.com

[S58] C++：命名空间
来源：http://kzy.guowangkeji.top

namespace ns { int f() { return 1; } }
来源：http://ebc.kuanghao11.cn

[S59] C++：静态断言
来源：http://fik.hysaishi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cyf.zycfv.cn

[S60] C++：遍历并删除元素
来源：http://lje.hnxiangtu.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qxv.dianchejie.cn

================================================================================
来源：http://wno.ctjpmb.com

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kvt.wangdashe.top

================================================================================
来源：http://wof.ybcxt.top


<!-- 参考信息 -->