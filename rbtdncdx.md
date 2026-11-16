代发 wailian999

R. Bash 专题
来源：http://arx.bjfxy.top

================================================================================
来源：http://alx.sxryk.cn

[R01] shebang 与严格模式
来源：http://ecb.vqdsnc.cn

#!/usr/bin/env bash
来源：http://uqg.tian-w.cn

set -euo pipefail
来源：http://nyv.mhx1999.top

[R02] 变量赋值与使用
来源：http://zmf.ybcxt.top

name="Tom"; echo "$name"
来源：http://fye.chenjidiqi.icu

[R03] 只读变量
来源：http://ino.cdnleiting.top

readonly PI=3.14
来源：http://wgo.birdmap.top

[R04] 位置参数
来源：http://hvl.pengpengdd.cyou

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cjx.fengsongda.top

[R05] 参数默认值
来源：http://jta.aizwys.cn

name="${1:-default}"
来源：http://nrd.cheryme.top

[R06] 判断命令是否存在
来源：http://cmv.9152youxi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kyk.cashguo.top

[R07] if 判断文件
来源：http://kyx.tanke756.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mtq.shzxlz.cn

[R08] 数值比较
来源：http://gge.zycfv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://zmt.yuxming.cn

[R09] 字符串比较
来源：http://ljw.uphjek.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sps.tarul.cn

[R10] 正则匹配
来源：http://tvp.wangshuangyany.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ubs.pengpengdd.cyou

[R11] case 多分支
来源：http://ekg.jinqigufen.top

case "$1" in
来源：http://dxx.ctjpmb.com

start) echo "启动" ;;
来源：http://jba.ctjpmb.com

stop)  echo "停止" ;;
来源：http://vyt.wangshuangyany.cn

*)     echo "未知命令" ;;
来源：http://nou.sweek.top

esac
来源：http://dnc.pycfn.com

[R12] for 遍历文件
来源：http://pwu.shangyingyoupin.top

for f in *.txt; do echo "$f"; done
来源：http://rgu.pycfn.com

[R13] for 计数循环
来源：http://uof.cheryme.top

for i in {1..10}; do echo "$i"; done
来源：http://ccd.nwbrower.top

[R14] C 风格 for
来源：http://goi.hesvh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yow.yanxiufei.cn

[R15] while 逐行读文件
来源：http://hqd.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jwn.jlsjyb.cn

[R16] until 等待条件
来源：http://usu.jyoumei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vif.hesvh.cn

[R17] 数组定义与取值
来源：http://mew.ctjpmb.com

arr=(a b c); echo "${arr[0]}"
来源：http://hdx.tarul.cn

[R18] 遍历数组
来源：http://gno.ydjk.org.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pvj.hnqzz.top

[R19] 数组长度
来源：http://xpn.zhengqikj.top

echo "${#arr[@]}"
来源：http://vxd.guannengcc.top

[R20] 关联数组（字典）
来源：http://kyu.wangdashe.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://lvd.fanxiaobao.xyz

[R21] 字符串长度
来源：http://ewy.daria6918.cn

echo "${#s}"
来源：http://oiz.jyoumei.cn

[R22] 截取子串
来源：http://urt.gaohongyu789.top

echo "${s:0:5}"
来源：http://kgi.chenzaomai.com

[R23] 字符串替换
来源：http://lfe.yvedp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ttu.tian-w.cn

[R24] 大小写转换
来源：http://mgh.cdnleiting.top

echo "${s^^}"; echo "${s,,}"
来源：http://mrf.dashuyun.cn

[R25] 去后缀 / 去前缀
来源：http://ydc.pengpengdd.cyou

echo "${f%.txt}"; echo "${f#./}"
来源：http://ooa.shzxlz.cn

[R26] 命令替换
来源：http://brd.svipenyu.cn

now=$(date +%F); echo "$now"
来源：http://opu.yfazqb.com

[R27] 算术展开
来源：http://qfa.fanxiaobao.xyz

echo $((1 + 2 * 3))
来源：http://lgz.smart0.xyz

[R28] 浮点运算
来源：http://mkb.dianchejie.cn

echo "scale=2; 10/3" | bc
来源：http://mzg.fehbvm.com

[R29] 定义函数
来源：http://sbd.kuanghao11.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://slg.0kj1m.cn

[R30] 函数返回状态码
来源：http://pvc.mhx1999.top

f() { return 0; }; f || echo "失败了"
来源：http://rop.yj20258.top

[R31] 局部变量
来源：http://fus.hammf.cn

f() { local x=1; echo "$x"; }
来源：http://bic.hcnkem.com

[R32] 参数个数校验
来源：http://ycp.jinqigufen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gcs.jianghu66.top

[R33] 捕获错误并提示行号
来源：http://bob.shanyushiyangtech.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://nml.yj202588.top

[R34] 退出时清理
来源：http://xgw.xingfuxueyuan.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://qas.svipenyu.cn

[R35] 后台执行并等待
来源：http://dnp.dashuyun.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pcz.yuanzhike.top

[R36] 并发执行多个任务
来源：http://lxn.wangshuangyany.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://utx.redwolf501.top

[R37] 把输出赋给变量
来源：http://kgo.ybcxt.top

files=$(ls -1)
来源：http://jhl.aizwys.cn

[R38] 管道串联
来源：http://psg.hywenlv.cn

cat a.txt | grep -i error | wc -l
来源：http://ccy.fzhhl.top

[R39] 重定向标准输出与错误
来源：http://dno.fanxiaobao.xyz

cmd > out.log 2>&1
来源：http://chy.guowangkeji.top

[R40] 追加写日志
来源：http://uaf.yuxming.cn

echo "log" >> out.log
来源：http://jeq.jqgfzy.top

[R41] 丢弃输出
来源：http://zjf.shzxlz.cn

cmd >/dev/null 2>&1
来源：http://qir.hesvh.cn

[R42] 输入重定向
来源：http://ynf.ybcxt.top

wc -l < a.txt
来源：http://yow.ydzc1.top

[R43] 按名字查找文件
来源：http://qmt.nanxinkj.top

find . -name "*.log" -type f
来源：http://efl.hysaishi.cn

[R44] 按修改时间查找
来源：http://zbr.zhoulong.xyz

find . -mtime -7 -type f
来源：http://ihg.hnqzz.top

[R45] 批量删除
来源：http://gjk.ivvv.top

find . -name "*.tmp" -delete
来源：http://pbk.yvedp.cn

[R46] 递归替换文件内容
来源：http://ykl.xuanzx.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ajq.shanyushiyangkeji.top

[R47] sed 单行替换
来源：http://zlq.xinyue.icu

sed -i 's/foo/bar/g' a.txt
来源：http://zyz.mhx1999.top

[R48] awk 取指定列
来源：http://kca.chenzaomai.com

awk '{print $1, $3}' a.txt
来源：http://gbd.redwolf501.top

[R49] awk 带条件
来源：http://yge.xingfuxueyuan.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wlc.xylfe.cn

[R50] awk 求和
来源：http://muw.sufxvd.cn

awk '{s += $2} END {print s}' a.txt
来源：http://atk.zhixingplan.top

[R51] 排序去重取前几
来源：http://vge.hongshengwenyu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://jdj.fktsv.cn

[R52] 统计行数
来源：http://npp.cashguo.top

wc -l a.txt
来源：http://oip.sweek.top

[R53] 查看文件头与实时尾
来源：http://pbd.feifeiyinyue.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://njm.wangshuangyany.cn

[R54] 比较两个文件
来源：http://ztt.chenjidiqi.icu

diff a.txt b.txt
来源：http://ctb.fktsv.cn

[R55] 压缩与解压
来源：http://cty.ybcxt.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yon.shuidangran.top

[R56] 远程拷贝
来源：http://tse.yuanzhike.top

scp file user@host:/path/
来源：http://lrz.shangyingyoupin.top

[R57] 远程执行命令
来源：http://odk.yonumen.top

ssh user@host 'uptime'
来源：http://hdb.guowangkeji.top

[R58] 下载文件
来源：http://zvv.9152youxi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zfh.yonumen.top

[R59] 发 POST JSON
来源：http://ubh.fengsongda.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://you.ydzc1.top

[R60] 只看 HTTP 状态码
来源：http://fyp.jinyuanbaomall.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nnh.xylfe.cn

[R61] 磁盘占用
来源：http://ewm.vehdjk.com

df -h;  du -sh *
来源：http://pgk.xylfe.cn

[R62] 找最占空间的文件
来源：http://qjg.yvedp.cn

du -ah . | sort -rh | head -10
来源：http://vuc.mhx1999.top

[R63] 内存与进程
来源：http://dhz.yj20258.top

free -h;  ps aux | grep nginx
来源：http://czx.zhongyouzk.top

[R64] 结束进程
来源：http://frh.fzhhl.top

kill -9 $(pgrep -f app.py)
来源：http://buv.ywan-chungtsiang.top

[R65] 查看端口占用
来源：http://esq.ydzc1.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dcc.hongshengwenyu.top

[R66] 定时任务
来源：http://ziz.kuanghao11.cn

crontab -e;  crontab -l
来源：http://vor.fktsv.cn

[R67] 生成随机十六进制串
来源：http://lhq.ydjk.org.cn

openssl rand -hex 16
来源：http://uca.xylfe.cn

[R68] 计算文件校验值
来源：http://izz.shangyingyoupin.top

sha256sum a.txt;  md5sum a.txt
来源：http://gyy.jinghuilouyu.cn

[R69] 生成随机密码
来源：http://nde.hcnkem.com

head -c 16 /dev/urandom | base64
来源：http://wtk.cashguo.top

[R70] 时间戳与互转
来源：http://yqp.pengpengdd.cyou

date +%s;  date -d @1700000000
来源：http://ktz.c1oappe.top

[R71] 日期格式化
来源：http://cvd.bjfxy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://acw.shuidangran.top

[R72] 等待端口就绪
来源：http://jkl.yangfankeji.com

until nc -z localhost 3306; do sleep 1; done
来源：http://cks.shanyushiyangkeji.top

[R73] 分割大日志
来源：http://ghq.daria6918.cn

split -l 1000 big.log part_
来源：http://okt.zhoulong.xyz

[R74] 批量重命名
来源：http://fxz.hnxiangtu.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://svi.fktsv.cn

[R75] 导出环境变量
来源：http://ovi.zdbjq.cn

export PATH="$HOME/bin:$PATH"
来源：http://pfk.vehdjk.com

[R76] 使用临时文件
来源：http://dzy.zhiwuduotai.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://sfj.ywan-chungtsiang.top

[R77] 读取用户输入
来源：http://npf.daxiang520.top

read -rp "请输入: " ans
来源：http://jda.smart0.xyz

[R78] 交互式菜单
来源：http://ipr.guowangkeji.top

select opt in a b c; do echo "$opt"; break; done
来源：http://plm.meibo888.top

[R79] 解析命令行选项
来源：http://fiq.fktsv.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bee.gaohongyu789.top

[R80] 查看脚本执行耗时
来源：http://hnx.bbcook.cn

time ./run.sh
来源：http://krh.pengpengdd.cyou

================================================================================
来源：http://pfp.andypj.xyz

S. C / C++ 专题
来源：http://hmi.chenzaomai.com

================================================================================
来源：http://fet.smart0.xyz

[S01] C：Hello World
来源：http://wyt.tianlin.xyz

#include <stdio.h>
来源：http://zuk.jyoumei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://stt.jinqigufen.top

[S02] C：变量与格式化输出
来源：http://pos.sufxvd.cn

int a = 10; printf("%d\n", a);
来源：http://ksd.shuidangran.top

[S03] C：读入整数
来源：http://awa.shuidangran.top

int x; scanf("%d", &x);
来源：http://yea.9152youxi.cn

[S04] C：字符串复制
来源：http://mos.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://nxu.cdnleiting.top

[S05] C：字符串长度
来源：http://eox.zdqjudy.top

strlen(s)
来源：http://nxi.jinqigfzy.top

[S06] C：字符串比较
来源：http://too.yongpay.top

strcmp(a, b) == 0
来源：http://res.bjfxy.top

[S07] C：数组遍历求和
来源：http://arp.snrcjt.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hpa.cucudq.cn

[S08] C：动态内存分配与释放
来源：http://bsu.jinghuilouyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aps.yongpay.top

[S09] C：结构体定义与初始化
来源：http://gcr.chenzaomai.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cqt.yanxiufei.cn

[S10] C：指针与解引用
来源：http://tme.jqgfzy.top

int *p = &a;  *p = 5;
来源：http://xlo.redwolf501.top

[S11] C：逐行读文件
来源：http://kaz.hfpthk.cn

FILE *f = fopen("a.txt", "r");
来源：http://pix.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xuz.tian-w.cn

fclose(f);
来源：http://zun.yanxiufei.cn

[S12] C：写文件
来源：http://ifk.sjlbkw.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xkl.hfpthk.cn

[S13] C：宏定义
来源：http://vvi.fehbvm.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xck.9152youxi.cn

[S14] C：枚举
来源：http://sge.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://ybo.fktsv.cn

[S15] C：类型转换
来源：http://fzw.jianghu66.top

(double) a / b
来源：http://tkz.cheryme.top

[S16] C：位操作置位
来源：http://kqh.yj20258888.top

x |= (1 << 3);
来源：http://jjg.52xcode.cn

[S17] C：安全拼接字符串
来源：http://mpi.havefunace.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mlz.svipenyu.cn

[S18] C：命令行参数
来源：http://wef.jyoumei.cn

int main(int argc, char **argv)
来源：http://erj.andypj.xyz

[S19] C：快速排序
来源：http://wfu.zdbjq.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fmx.jqgufenzy.top

[S20] C：二分查找
来源：http://owr.snrcjt.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ynt.xziqi.cn

[S21] C：字符类别判断
来源：http://iki.ppjwa.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://izo.hysaishi.cn

[S22] C：字符串转数字
来源：http://waw.kuanghao11.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sum.feifeiyinyue.top

[S23] C：随机数
来源：http://yvp.c1oappe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://abk.fktsv.cn

[S24] C：获取本地时间
来源：http://jal.yongpay.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ruv.wangshuangyany.cn

[S25] C：内存拷贝
来源：http://ity.chenzaomai.com

memcpy(dst, src, n);
来源：http://exp.cucudq.cn

[S26] C：内存清零
来源：http://whp.pycfn.com

memset(a, 0, sizeof a);
来源：http://bnd.zhoulong.xyz

[S27] C：定义常量
来源：http://mgc.fktsv.cn

const double PI = 3.14159;
来源：http://hlr.pengpengdd.cyou

[S28] C：静态变量
来源：http://wfm.tian-w.cn

static int counter = 0;
来源：http://akt.wangdashe.top

[S29] C：变参函数
来源：http://jhy.shuidangran.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ecx.gzhubu.top

[S30] C：头文件保护
来源：http://jau.epnwcf.com

#ifndef X_H
来源：http://ooc.cashguo.top

#define X_H
来源：http://bon.jinghuilouyu.cn

#endif
来源：http://hgv.hesvh.cn

[S31] C++：Hello World
来源：http://fqx.ivvv.top

#include <iostream>
来源：http://wgm.9152youxi.cn

int main() { std::cout << "Hello\n"; }
来源：http://cjt.birdmap.top

[S32] C++：字符串
来源：http://imk.hfpthk.cn

std::string s = "hi";  s += "!";
来源：http://uxs.jlsjyb.cn

[S33] C++：vector 增删
来源：http://tno.haohaochexian.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://apu.ehwqpu.com

[S34] C++：遍历 vector
来源：http://wwq.jianghu66.top

for (auto &x : v) { std::cout << x; }
来源：http://odv.yuxming.cn

[S35] C++：map
来源：http://ymo.jqgfzy.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jyk.yj202588.top

[S36] C++：unordered_map
来源：http://sby.0kj1m.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dau.yonumen.top

[S37] C++：set
来源：http://qna.jqgfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zle.bjfxy.top

[S38] C++：排序
来源：http://xuf.nanxuanxn.top

std::sort(v.begin(), v.end());
来源：http://pmx.yueranfly.top

[S39] C++：自定义比较器排序
来源：http://daa.snrcjt.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kej.havefunace.top

[S40] C++：查找元素
来源：http://pdy.jinyuanbaomall.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ucj.pengpengdd.cyou

[S41] C++：类与构造函数
来源：http://eqp.nanxinkj.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rox.zdqjudy.top

[S42] C++：继承与虚函数
来源：http://kvf.jinqigfzy.top

class B : public Base { public: void f() override {} };
来源：http://pvu.daxiang520.top

[S43] C++：智能指针
来源：http://djz.iojbl.cn

auto p = std::make_unique<int>(5);
来源：http://ect.havefunace.top

[S44] C++：引用传参
来源：http://igc.yuxming.cn

void inc(int &x) { ++x; }
来源：http://wvs.ehwqpu.com

[S45] C++：lambda
来源：http://phi.wangdashe.top

auto add = [](int a, int b) { return a + b; };
来源：http://mwj.yanxiufei.cn

[S46] C++：函数模板
来源：http://kzj.yuxming.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jvh.zhaomingkeji.xyz

[S47] C++：结构化绑定遍历
来源：http://imz.zhaomingkeji.xyz

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wgc.xylfe.cn

[S48] C++：逐行读文件
来源：http://acg.xziqi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://juq.smart0.xyz

while (std::getline(in, line)) { }
来源：http://pav.shuidangran.top

[S49] C++：写文件
来源：http://fns.zdqjudy.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cza.fanxiaobao.xyz

[S50] C++：格式化数字
来源：http://kge.meibo888.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kpk.shanyushiyangkeji.top

[S51] C++：显式类型转换
来源：http://fdv.sweek.top

static_cast<double>(a) / b
来源：http://ker.fzhhl.top

[S52] C++：const 与 noexcept
来源：http://eao.c1oappe.top

int size() const noexcept { return n_; }
来源：http://chy.guowangkeji.top

[S53] C++：移动语义
来源：http://uvh.vehdjk.com

std::vector<int> w = std::move(v);
来源：http://xaj.yj20258888.top

[S54] C++：异常处理
来源：http://cgn.nanxinkj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wdy.ivvv.top

[S55] C++：结构化绑定
来源：http://tib.feifeiyinyue.top

auto [a, b] = std::make_pair(1, 2);
来源：http://fjr.shzxlz.cn

[S56] C++：optional
来源：http://ujr.ydjk.org.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mow.chenzaomai.com

[S57] C++：编译期常量
来源：http://xlw.tarul.cn

constexpr int N = 10;
来源：http://mpn.jyoumei.cn

[S58] C++：命名空间
来源：http://cad.dashuyun.cn

namespace ns { int f() { return 1; } }
来源：http://jgq.cucudq.cn

[S59] C++：静态断言
来源：http://obk.aibaodan.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dir.yanxiufei.cn

[S60] C++：遍历并删除元素
来源：http://ffy.mhx1999.top

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ply.shanyushiyangtech.top

================================================================================
来源：http://hou.haohaochexian.top

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cdy.tianlin.xyz

================================================================================
来源：http://vij.cheryme.top


<!-- 参考信息 -->