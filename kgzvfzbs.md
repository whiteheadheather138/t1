代发 wailian999

R. Bash 专题
来源：http://yke.aibaodan.cn

================================================================================
来源：http://juw.xinyue.icu

[R01] shebang 与严格模式
来源：http://dtb.zhixingplan.top

#!/usr/bin/env bash
来源：http://pig.hfpthk.cn

set -euo pipefail
来源：http://rnw.ivvv.top

[R02] 变量赋值与使用
来源：http://fzk.zhoulong.xyz

name="Tom"; echo "$name"
来源：http://ton.tian-w.cn

[R03] 只读变量
来源：http://fga.snrcjt.cn

readonly PI=3.14
来源：http://qkw.zhongyouzk.top

[R04] 位置参数
来源：http://yvp.zhongyouzk.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cuw.52xcode.cn

[R05] 参数默认值
来源：http://goc.wangshuangyany.cn

name="${1:-default}"
来源：http://nph.yj20258888.top

[R06] 判断命令是否存在
来源：http://hdm.havefunace.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sgj.hnqzz.top

[R07] if 判断文件
来源：http://unc.yuxming.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://evx.wangdashe.top

[R08] 数值比较
来源：http://qcv.ybcxt.top

if (( a > b )); then echo "a 更大"; fi
来源：http://wpx.yangfankeji.com

[R09] 字符串比较
来源：http://ckl.pengpengdd.cyou

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://iob.cqqwz.cn

[R10] 正则匹配
来源：http://mrv.xingfuxueyuan.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://obe.yj202588.top

[R11] case 多分支
来源：http://dfm.daria6918.cn

case "$1" in
来源：http://cqd.shuidangran.top

start) echo "启动" ;;
来源：http://yah.zdqjudy.top

stop)  echo "停止" ;;
来源：http://eve.316326.xyz

*)     echo "未知命令" ;;
来源：http://xlb.fanxiaobao.xyz

esac
来源：http://bkd.daxiang520.top

[R12] for 遍历文件
来源：http://dsn.xziqi.cn

for f in *.txt; do echo "$f"; done
来源：http://jdz.smart0.xyz

[R13] for 计数循环
来源：http://zov.ppjwa.cn

for i in {1..10}; do echo "$i"; done
来源：http://svc.316326.xyz

[R14] C 风格 for
来源：http://eue.ctjpmb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jyr.jiagoushi.top

[R15] while 逐行读文件
来源：http://vnj.jianghu66.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://uui.guannengcc.top

[R16] until 等待条件
来源：http://bje.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xry.tianlin.xyz

[R17] 数组定义与取值
来源：http://ght.andypj.xyz

arr=(a b c); echo "${arr[0]}"
来源：http://mgb.meibo888.top

[R18] 遍历数组
来源：http://bwf.vehdjk.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hwa.daria6918.cn

[R19] 数组长度
来源：http://ehs.cashguo.top

echo "${#arr[@]}"
来源：http://ila.fktsv.cn

[R20] 关联数组（字典）
来源：http://swa.fktsv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bna.cheryme.top

[R21] 字符串长度
来源：http://rof.cqqwz.cn

echo "${#s}"
来源：http://qae.xziqi.cn

[R22] 截取子串
来源：http://vmw.tarul.cn

echo "${s:0:5}"
来源：http://lys.sufxvd.cn

[R23] 字符串替换
来源：http://jdf.chenzaomai.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://rnh.mhx1999.top

[R24] 大小写转换
来源：http://sgz.epnwcf.com

echo "${s^^}"; echo "${s,,}"
来源：http://mes.hesvh.cn

[R25] 去后缀 / 去前缀
来源：http://uxa.jinghuilouyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lya.fanxiaobao.xyz

[R26] 命令替换
来源：http://ebi.jinqigufen.top

now=$(date +%F); echo "$now"
来源：http://vai.yuanzhike.top

[R27] 算术展开
来源：http://ycs.chenjidiqi.icu

echo $((1 + 2 * 3))
来源：http://khv.pengpengdd.cyou

[R28] 浮点运算
来源：http://npe.nwbrower.top

echo "scale=2; 10/3" | bc
来源：http://uox.kuanghao11.cn

[R29] 定义函数
来源：http://bqz.vqdsnc.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://jrw.jianghu66.top

[R30] 函数返回状态码
来源：http://zkc.xinyue.icu

f() { return 0; }; f || echo "失败了"
来源：http://tnj.cashguo.top

[R31] 局部变量
来源：http://vmm.jlsjyb.cn

f() { local x=1; echo "$x"; }
来源：http://zcr.cucudq.cn

[R32] 参数个数校验
来源：http://fos.chenzaomai.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://emz.zdbjq.cn

[R33] 捕获错误并提示行号
来源：http://kuh.snrcjt.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ano.dashuyun.cn

[R34] 退出时清理
来源：http://ysv.ivvv.top

trap 'rm -f "$tmp"' EXIT
来源：http://hmj.xingfuxueyuan.xyz

[R35] 后台执行并等待
来源：http://nsm.ywan-chungtsiang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fjd.jianghu66.top

[R36] 并发执行多个任务
来源：http://dki.jyoumei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jvo.fanxiaobao.xyz

[R37] 把输出赋给变量
来源：http://jes.fengsongda.top

files=$(ls -1)
来源：http://izm.yvedp.cn

[R38] 管道串联
来源：http://aer.yj202588.top

cat a.txt | grep -i error | wc -l
来源：http://usx.aizwys.cn

[R39] 重定向标准输出与错误
来源：http://dea.gaohongyu789.top

cmd > out.log 2>&1
来源：http://pxn.pycfn.com

[R40] 追加写日志
来源：http://mea.jqgufenzy.top

echo "log" >> out.log
来源：http://zxf.andypj.xyz

[R41] 丢弃输出
来源：http://opj.svipenyu.cn

cmd >/dev/null 2>&1
来源：http://cst.zhijiandao.cn

[R42] 输入重定向
来源：http://ujo.jiagoushi.top

wc -l < a.txt
来源：http://vnp.jianghu66.top

[R43] 按名字查找文件
来源：http://ubh.yanxiufei.cn

find . -name "*.log" -type f
来源：http://bpb.shanyushiyangtech.top

[R44] 按修改时间查找
来源：http://ipv.yvedp.cn

find . -mtime -7 -type f
来源：http://etp.yueranfly.top

[R45] 批量删除
来源：http://ujm.nwbrower.top

find . -name "*.tmp" -delete
来源：http://pdr.hongshengwenyu.top

[R46] 递归替换文件内容
来源：http://wry.yanxiufei.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://sbb.ehwqpu.com

[R47] sed 单行替换
来源：http://xmh.svipenyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rbv.zhixingplan.top

[R48] awk 取指定列
来源：http://hji.wangdashe.top

awk '{print $1, $3}' a.txt
来源：http://clc.cheryme.top

[R49] awk 带条件
来源：http://mom.birdmap.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jsn.sufxvd.cn

[R50] awk 求和
来源：http://ipr.c1oappe.top

awk '{s += $2} END {print s}' a.txt
来源：http://ull.zhixingplan.top

[R51] 排序去重取前几
来源：http://ftj.zhoulong.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://veb.hysaishi.cn

[R52] 统计行数
来源：http://dpb.epnwcf.com

wc -l a.txt
来源：http://xaq.cqqwz.cn

[R53] 查看文件头与实时尾
来源：http://mwu.meibo888.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uxt.yvedp.cn

[R54] 比较两个文件
来源：http://oba.ydjk.org.cn

diff a.txt b.txt
来源：http://ozl.fktsv.cn

[R55] 压缩与解压
来源：http://qpz.bjfxy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://egg.yonumen.top

[R56] 远程拷贝
来源：http://uth.zhaomingkeji.xyz

scp file user@host:/path/
来源：http://zmo.hesvh.cn

[R57] 远程执行命令
来源：http://zvb.shanyushiyangtech.top

ssh user@host 'uptime'
来源：http://uni.xuanzx.com

[R58] 下载文件
来源：http://wvo.chenzaomai.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fpq.yangfankeji.com

[R59] 发 POST JSON
来源：http://znf.gotoacloud.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://buk.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://rsj.aizwys.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rij.gaohongyu789.top

[R61] 磁盘占用
来源：http://bah.snrcjt.cn

df -h;  du -sh *
来源：http://mkl.smart0.xyz

[R62] 找最占空间的文件
来源：http://ycm.hammf.cn

du -ah . | sort -rh | head -10
来源：http://qed.hammf.cn

[R63] 内存与进程
来源：http://hit.aibaodan.cn

free -h;  ps aux | grep nginx
来源：http://lte.guannengcc.top

[R64] 结束进程
来源：http://gws.sufxvd.cn

kill -9 $(pgrep -f app.py)
来源：http://wck.zdqjudy.top

[R65] 查看端口占用
来源：http://fai.redwolf501.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mnk.xingfuxueyuan.xyz

[R66] 定时任务
来源：http://sae.wangdashe.top

crontab -e;  crontab -l
来源：http://tuo.uphjek.com

[R67] 生成随机十六进制串
来源：http://bxs.feifeiyinyue.top

openssl rand -hex 16
来源：http://uhx.daxiang520.top

[R68] 计算文件校验值
来源：http://qzl.hfpthk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://hou.birdmap.top

[R69] 生成随机密码
来源：http://hhj.jiagoushi.top

head -c 16 /dev/urandom | base64
来源：http://gpt.hfpthk.cn

[R70] 时间戳与互转
来源：http://ooz.zhoulong.xyz

date +%s;  date -d @1700000000
来源：http://gex.chenzaomai.com

[R71] 日期格式化
来源：http://zzv.nanxinkj.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kht.chenlongwang.top

[R72] 等待端口就绪
来源：http://vbo.zhijiandao.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://auy.yanxiufei.cn

[R73] 分割大日志
来源：http://fua.ctjpmb.com

split -l 1000 big.log part_
来源：http://wla.ivvv.top

[R74] 批量重命名
来源：http://tba.jyoumei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rhe.0kj1m.cn

[R75] 导出环境变量
来源：http://vju.dianchejie.cn

export PATH="$HOME/bin:$PATH"
来源：http://pgu.jqgfzy.top

[R76] 使用临时文件
来源：http://uoc.hesvh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vvu.shanyushiyangkeji.top

[R77] 读取用户输入
来源：http://qvu.xylfe.cn

read -rp "请输入: " ans
来源：http://vne.yuxming.cn

[R78] 交互式菜单
来源：http://mjv.smart0.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://ymt.ivvv.top

[R79] 解析命令行选项
来源：http://zun.gzhubu.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tbj.shanyushiyangtech.top

[R80] 查看脚本执行耗时
来源：http://nvl.yj202588.top

time ./run.sh
来源：http://war.yj20258888.top

================================================================================
来源：http://scw.cdnleiting.top

S. C / C++ 专题
来源：http://qzo.ctjpmb.com

================================================================================
来源：http://asn.ywan-chungtsiang.top

[S01] C：Hello World
来源：http://eca.yongpay.top

#include <stdio.h>
来源：http://jar.chenjidiqi.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://iym.epnwcf.com

[S02] C：变量与格式化输出
来源：http://cdx.zdqjudy.top

int a = 10; printf("%d\n", a);
来源：http://itp.jlsjyb.cn

[S03] C：读入整数
来源：http://mra.xinyue.icu

int x; scanf("%d", &x);
来源：http://zpx.c1oappe.top

[S04] C：字符串复制
来源：http://yyz.fehbvm.com

char dst[32]; strcpy(dst, "hi");
来源：http://enh.jinqigufen.top

[S05] C：字符串长度
来源：http://ayr.fehbvm.com

strlen(s)
来源：http://viw.yueranfly.top

[S06] C：字符串比较
来源：http://bay.cheryme.top

strcmp(a, b) == 0
来源：http://kcl.sjlbkw.cn

[S07] C：数组遍历求和
来源：http://gcb.aibaodan.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pmr.tian-w.cn

[S08] C：动态内存分配与释放
来源：http://ujc.bbcook.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sdi.andypj.xyz

[S09] C：结构体定义与初始化
来源：http://zxe.jinyuanbaomall.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gvq.jinqigfzy.top

[S10] C：指针与解引用
来源：http://dbi.tianlin.xyz

int *p = &a;  *p = 5;
来源：http://nnv.yj20258.top

[S11] C：逐行读文件
来源：http://emi.uphjek.com

FILE *f = fopen("a.txt", "r");
来源：http://ado.dashuyun.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pmj.gaohongyu789.top

fclose(f);
来源：http://jsj.dashuyun.cn

[S12] C：写文件
来源：http://eqq.shzxlz.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tux.sysykeji.top

[S13] C：宏定义
来源：http://krc.0kj1m.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hpv.haohaochexian.top

[S14] C：枚举
来源：http://eis.xziqi.cn

enum Color { RED, GREEN, BLUE };
来源：http://ljj.tian-w.cn

[S15] C：类型转换
来源：http://xpc.yj20258888.top

(double) a / b
来源：http://lon.svipenyu.cn

[S16] C：位操作置位
来源：http://jgl.daria6918.cn

x |= (1 << 3);
来源：http://hvy.zhengqikj.top

[S17] C：安全拼接字符串
来源：http://mig.shuidangran.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tlo.redwolf501.top

[S18] C：命令行参数
来源：http://pix.hcnkem.com

int main(int argc, char **argv)
来源：http://bqw.pengpengdd.cyou

[S19] C：快速排序
来源：http://tas.zhoulong.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://oqy.chenlongwang.top

[S20] C：二分查找
来源：http://eaq.aizwys.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fbo.epnwcf.com

[S21] C：字符类别判断
来源：http://nvm.nwbrower.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zri.uphjek.com

[S22] C：字符串转数字
来源：http://nzo.hesvh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://pmu.hysaishi.cn

[S23] C：随机数
来源：http://hly.andypj.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://wem.zhengqikj.top

[S24] C：获取本地时间
来源：http://jgn.daria6918.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fqv.ybcxt.top

[S25] C：内存拷贝
来源：http://xli.fehbvm.com

memcpy(dst, src, n);
来源：http://hwd.xziqi.cn

[S26] C：内存清零
来源：http://aeo.nwbrower.top

memset(a, 0, sizeof a);
来源：http://wgn.uphjek.com

[S27] C：定义常量
来源：http://fqx.ywan-chungtsiang.top

const double PI = 3.14159;
来源：http://adg.hnqzz.top

[S28] C：静态变量
来源：http://lnm.jinqigufen.top

static int counter = 0;
来源：http://pqu.0kj1m.cn

[S29] C：变参函数
来源：http://sye.yongpay.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://caa.dashuyun.cn

[S30] C：头文件保护
来源：http://pnx.dianchejie.cn

#ifndef X_H
来源：http://xjf.hysaishi.cn

#define X_H
来源：http://qkw.zycfv.cn

#endif
来源：http://nqy.shanyushiyangtech.top

[S31] C++：Hello World
来源：http://ami.shanyushiyangtech.top

#include <iostream>
来源：http://gkn.yuxming.cn

int main() { std::cout << "Hello\n"; }
来源：http://asj.fehbvm.com

[S32] C++：字符串
来源：http://rpx.zhiwuduotai.top

std::string s = "hi";  s += "!";
来源：http://vry.xuetiantiany.cn

[S33] C++：vector 增删
来源：http://qgn.yonumen.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ujc.yvedp.cn

[S34] C++：遍历 vector
来源：http://rtn.zhoulong.xyz

for (auto &x : v) { std::cout << x; }
来源：http://dmf.xingfuxueyuan.xyz

[S35] C++：map
来源：http://kmz.wangdashe.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kij.iojbl.cn

[S36] C++：unordered_map
来源：http://cpv.shuidangran.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qdz.hysaishi.cn

[S37] C++：set
来源：http://pdo.fengsongda.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vxy.ybcxt.top

[S38] C++：排序
来源：http://emr.yj20258.top

std::sort(v.begin(), v.end());
来源：http://ozx.ywan-chungtsiang.top

[S39] C++：自定义比较器排序
来源：http://yco.hywenlv.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vqk.cheryme.top

[S40] C++：查找元素
来源：http://btv.wangdashe.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://vjb.jlsjyb.cn

[S41] C++：类与构造函数
来源：http://akh.dianchejie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://anq.pengpengdd.cyou

[S42] C++：继承与虚函数
来源：http://woq.kuanghao11.cn

class B : public Base { public: void f() override {} };
来源：http://mjk.yuxming.cn

[S43] C++：智能指针
来源：http://frk.cucudq.cn

auto p = std::make_unique<int>(5);
来源：http://rtp.feifeiyinyue.top

[S44] C++：引用传参
来源：http://mxg.zhoulong.xyz

void inc(int &x) { ++x; }
来源：http://qef.ydjk.org.cn

[S45] C++：lambda
来源：http://tye.yangfankeji.com

auto add = [](int a, int b) { return a + b; };
来源：http://gfl.zhiwuduotai.top

[S46] C++：函数模板
来源：http://lqv.nanxuanxn.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gcx.aibaodan.cn

[S47] C++：结构化绑定遍历
来源：http://ieu.yj202588.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://kxq.nanxuanxn.top

[S48] C++：逐行读文件
来源：http://ore.tanke756.top

std::ifstream in("a.txt");  std::string line;
来源：http://kpn.sweek.top

while (std::getline(in, line)) { }
来源：http://crt.shanyushiyangkeji.top

[S49] C++：写文件
来源：http://uzk.epnwcf.com

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wjl.sysykeji.top

[S50] C++：格式化数字
来源：http://ztv.ctjpmb.com

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://czu.sweek.top

[S51] C++：显式类型转换
来源：http://oia.shzxlz.cn

static_cast<double>(a) / b
来源：http://jon.andypj.xyz

[S52] C++：const 与 noexcept
来源：http://rwk.nanxinkj.top

int size() const noexcept { return n_; }
来源：http://ooi.aizwys.cn

[S53] C++：移动语义
来源：http://nao.kuanghao11.cn

std::vector<int> w = std::move(v);
来源：http://etd.c1oappe.top

[S54] C++：异常处理
来源：http://ucx.tian-w.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vrb.hongshengwenyu.top

[S55] C++：结构化绑定
来源：http://vor.haohaochexian.top

auto [a, b] = std::make_pair(1, 2);
来源：http://bue.xylfe.cn

[S56] C++：optional
来源：http://bde.yongpay.top

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vau.zhijiandao.cn

[S57] C++：编译期常量
来源：http://kgq.jinghuilouyu.cn

constexpr int N = 10;
来源：http://lyh.yuxming.cn

[S58] C++：命名空间
来源：http://laa.zhengqikj.top

namespace ns { int f() { return 1; } }
来源：http://qus.jinqigfzy.top

[S59] C++：静态断言
来源：http://jav.cdnleiting.top

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kpa.0kj1m.cn

[S60] C++：遍历并删除元素
来源：http://cts.yonumen.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://plc.tian-w.cn

================================================================================
来源：http://rpf.snrcjt.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mqs.zhijiandao.cn

================================================================================
来源：http://res.fengsongda.top


<!-- 参考信息 -->