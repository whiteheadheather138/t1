代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://igi.ctjpmb.com

[Q90] 生成序号列
来源：http://ykf.xylfe.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://joa.sxryk.cn

================================================================================
来源：http://tym.ydzc1.top

R. Bash 专题
来源：http://osq.ctjpmb.com

================================================================================
来源：http://hgj.hnqzz.top

[R01] shebang 与严格模式
来源：http://tad.mhx1999.top

#!/usr/bin/env bash
来源：http://kgs.dashuyun.cn

set -euo pipefail
来源：http://vvl.jianghu66.top

[R02] 变量赋值与使用
来源：http://irl.cheryme.top

name="Tom"; echo "$name"
来源：http://dqz.snrcjt.cn

[R03] 只读变量
来源：http://xwt.sufxvd.cn

readonly PI=3.14
来源：http://rtm.fanxiaobao.xyz

[R04] 位置参数
来源：http://ptg.sxryk.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yaz.hnxiangtu.top

[R05] 参数默认值
来源：http://rpz.c1oappe.top

name="${1:-default}"
来源：http://ntk.zdqjudy.top

[R06] 判断命令是否存在
来源：http://ddl.ywan-chungtsiang.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ahi.sysykeji.top

[R07] if 判断文件
来源：http://odk.jiagoushi.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oof.hywenlv.cn

[R08] 数值比较
来源：http://ajt.vehdjk.com

if (( a > b )); then echo "a 更大"; fi
来源：http://utn.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://hlu.vqdsnc.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://skg.nanxinkj.top

[R10] 正则匹配
来源：http://yjw.bbcook.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qxk.zycfv.cn

[R11] case 多分支
来源：http://tjn.yuanzhike.top

case "$1" in
来源：http://lrk.kuanghao11.cn

start) echo "启动" ;;
来源：http://aqv.jyoumei.cn

stop)  echo "停止" ;;
来源：http://wfj.quarkkingdee.top

*)     echo "未知命令" ;;
来源：http://ndd.vehdjk.com

esac
来源：http://knu.yangfankeji.com

[R12] for 遍历文件
来源：http://uze.epnwcf.com

for f in *.txt; do echo "$f"; done
来源：http://jzu.hysaishi.cn

[R13] for 计数循环
来源：http://dzv.zdqjudy.top

for i in {1..10}; do echo "$i"; done
来源：http://cnq.hongshengwenyu.top

[R14] C 风格 for
来源：http://rei.tian-w.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://cxi.guannengcc.top

[R15] while 逐行读文件
来源：http://stf.gaohongyu789.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oda.gotoacloud.top

[R16] until 等待条件
来源：http://sdo.shuidangran.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hzm.guowangkeji.top

[R17] 数组定义与取值
来源：http://lzd.hnxiangtu.top

arr=(a b c); echo "${arr[0]}"
来源：http://oro.cucudq.cn

[R18] 遍历数组
来源：http://usu.nanxinkj.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://jhk.fzhhl.top

[R19] 数组长度
来源：http://bwj.ehwqpu.com

echo "${#arr[@]}"
来源：http://vyp.wangshuangyany.cn

[R20] 关联数组（字典）
来源：http://kha.hfpthk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://tsw.pycfn.com

[R21] 字符串长度
来源：http://ugd.hongshengwenyu.top

echo "${#s}"
来源：http://rnt.uphjek.com

[R22] 截取子串
来源：http://and.guowangkeji.top

echo "${s:0:5}"
来源：http://agy.hesvh.cn

[R23] 字符串替换
来源：http://yeb.fanxiaobao.xyz

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qlp.ywan-chungtsiang.top

[R24] 大小写转换
来源：http://qog.yongpay.top

echo "${s^^}"; echo "${s,,}"
来源：http://hbb.ywan-chungtsiang.top

[R25] 去后缀 / 去前缀
来源：http://xff.zdqjudy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://cbo.quarkkingdee.top

[R26] 命令替换
来源：http://jhb.hesvh.cn

now=$(date +%F); echo "$now"
来源：http://icn.hnqzz.top

[R27] 算术展开
来源：http://dnt.jinghuilouyu.cn

echo $((1 + 2 * 3))
来源：http://wgp.ctjpmb.com

[R28] 浮点运算
来源：http://wtm.tanke756.top

echo "scale=2; 10/3" | bc
来源：http://yty.ydzc1.top

[R29] 定义函数
来源：http://ull.yfazqb.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gzy.yfazqb.com

[R30] 函数返回状态码
来源：http://npo.svipenyu.cn

f() { return 0; }; f || echo "失败了"
来源：http://ohr.dianchejie.cn

[R31] 局部变量
来源：http://llv.mhx1999.top

f() { local x=1; echo "$x"; }
来源：http://liq.havefunace.top

[R32] 参数个数校验
来源：http://ojj.wangshuangyany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rfy.zhixingplan.top

[R33] 捕获错误并提示行号
来源：http://iog.c1oappe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rhs.cheryme.top

[R34] 退出时清理
来源：http://sym.nwbrower.top

trap 'rm -f "$tmp"' EXIT
来源：http://bql.hesvh.cn

[R35] 后台执行并等待
来源：http://ewk.zhoulong.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://acn.meibo888.top

[R36] 并发执行多个任务
来源：http://epc.jqgufenzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xfo.chenzaomai.com

[R37] 把输出赋给变量
来源：http://xxb.hammf.cn

files=$(ls -1)
来源：http://sby.zhongyouzk.top

[R38] 管道串联
来源：http://yhx.mhx1999.top

cat a.txt | grep -i error | wc -l
来源：http://wat.svipenyu.cn

[R39] 重定向标准输出与错误
来源：http://nmi.yj20258.top

cmd > out.log 2>&1
来源：http://dvt.ywan-chungtsiang.top

[R40] 追加写日志
来源：http://iri.hywenlv.cn

echo "log" >> out.log
来源：http://nap.tarul.cn

[R41] 丢弃输出
来源：http://pmi.ppjwa.cn

cmd >/dev/null 2>&1
来源：http://sms.jinqigfzy.top

[R42] 输入重定向
来源：http://qpg.vehdjk.com

wc -l < a.txt
来源：http://zbb.hcnkem.com

[R43] 按名字查找文件
来源：http://qgw.gzhubu.top

find . -name "*.log" -type f
来源：http://npt.yuxming.cn

[R44] 按修改时间查找
来源：http://wie.cdnleiting.top

find . -mtime -7 -type f
来源：http://jij.sxryk.cn

[R45] 批量删除
来源：http://rej.cdnleiting.top

find . -name "*.tmp" -delete
来源：http://ayb.ehwqpu.com

[R46] 递归替换文件内容
来源：http://aui.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xzh.xingfuxueyuan.xyz

[R47] sed 单行替换
来源：http://wdx.snrcjt.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vul.yvedp.cn

[R48] awk 取指定列
来源：http://fxf.gzhubu.top

awk '{print $1, $3}' a.txt
来源：http://nno.0kj1m.cn

[R49] awk 带条件
来源：http://lgs.fktsv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yys.andypj.xyz

[R50] awk 求和
来源：http://qaz.xziqi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://npj.wangdashe.top

[R51] 排序去重取前几
来源：http://zlv.jlsjyb.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://wus.andypj.xyz

[R52] 统计行数
来源：http://cxb.yvedp.cn

wc -l a.txt
来源：http://xrq.fengsongda.top

[R53] 查看文件头与实时尾
来源：http://jtr.jinqigfzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rou.xuetiantiany.cn

[R54] 比较两个文件
来源：http://hfj.cucudq.cn

diff a.txt b.txt
来源：http://dqk.gotoacloud.top

[R55] 压缩与解压
来源：http://cua.ydjk.org.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://awd.tianlin.xyz

[R56] 远程拷贝
来源：http://bqc.chenzaomai.com

scp file user@host:/path/
来源：http://zai.havefunace.top

[R57] 远程执行命令
来源：http://sie.xuanzx.com

ssh user@host 'uptime'
来源：http://gqp.zhengqikj.top

[R58] 下载文件
来源：http://ozh.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oes.ybcxt.top

[R59] 发 POST JSON
来源：http://exg.tanke756.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vmj.ctjpmb.com

[R60] 只看 HTTP 状态码
来源：http://hbd.birdmap.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dce.mhx1999.top

[R61] 磁盘占用
来源：http://dek.jqgfzy.top

df -h;  du -sh *
来源：http://fdl.316326.xyz

[R62] 找最占空间的文件
来源：http://cyr.chenlongwang.top

du -ah . | sort -rh | head -10
来源：http://cin.zdbjq.cn

[R63] 内存与进程
来源：http://ugv.tarul.cn

free -h;  ps aux | grep nginx
来源：http://izo.hnxiangtu.top

[R64] 结束进程
来源：http://nkc.ctjpmb.com

kill -9 $(pgrep -f app.py)
来源：http://lcv.hcnkem.com

[R65] 查看端口占用
来源：http://oyw.hesvh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xqf.guannengcc.top

[R66] 定时任务
来源：http://ljt.wangshuangyany.cn

crontab -e;  crontab -l
来源：http://cvp.andypj.xyz

[R67] 生成随机十六进制串
来源：http://rny.ydjk.org.cn

openssl rand -hex 16
来源：http://njy.sysykeji.top

[R68] 计算文件校验值
来源：http://qjr.meibo888.top

sha256sum a.txt;  md5sum a.txt
来源：http://lde.shuidangran.top

[R69] 生成随机密码
来源：http://kdw.haohaochexian.top

head -c 16 /dev/urandom | base64
来源：http://kbc.yfazqb.com

[R70] 时间戳与互转
来源：http://fzu.cdnleiting.top

date +%s;  date -d @1700000000
来源：http://adx.fanxiaobao.xyz

[R71] 日期格式化
来源：http://tdy.vehdjk.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://atk.ywan-chungtsiang.top

[R72] 等待端口就绪
来源：http://ylm.snrcjt.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kaf.c1oappe.top

[R73] 分割大日志
来源：http://trf.cashguo.top

split -l 1000 big.log part_
来源：http://zwr.chenlongwang.top

[R74] 批量重命名
来源：http://zou.yueranfly.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sgt.feifeiyinyue.top

[R75] 导出环境变量
来源：http://psa.daria6918.cn

export PATH="$HOME/bin:$PATH"
来源：http://fjk.kuanghao11.cn

[R76] 使用临时文件
来源：http://ebw.yj20258888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ptk.mhx1999.top

[R77] 读取用户输入
来源：http://mah.zhijiandao.cn

read -rp "请输入: " ans
来源：http://glv.yvedp.cn

[R78] 交互式菜单
来源：http://dlr.vqdsnc.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://mhy.zycfv.cn

[R79] 解析命令行选项
来源：http://wvj.jlsjyb.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://smr.wangdashe.top

[R80] 查看脚本执行耗时
来源：http://jwh.xuanzx.com

time ./run.sh
来源：http://oac.hywenlv.cn

================================================================================
来源：http://hqk.hysaishi.cn

S. C / C++ 专题
来源：http://mlw.fanxiaobao.xyz

================================================================================
来源：http://pzy.xylfe.cn

[S01] C：Hello World
来源：http://bmq.xuanzx.com

#include <stdio.h>
来源：http://ouj.redwolf501.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ajx.jianghu66.top

[S02] C：变量与格式化输出
来源：http://hqs.gzhubu.top

int a = 10; printf("%d\n", a);
来源：http://ktj.meibo888.top

[S03] C：读入整数
来源：http://irw.tanke756.top

int x; scanf("%d", &x);
来源：http://nbk.chenjidiqi.icu

[S04] C：字符串复制
来源：http://jee.ivvv.top

char dst[32]; strcpy(dst, "hi");
来源：http://tje.yuanzhike.top

[S05] C：字符串长度
来源：http://dha.xuetiantiany.cn

strlen(s)
来源：http://thp.shanyushiyangkeji.top

[S06] C：字符串比较
来源：http://qzd.epnwcf.com

strcmp(a, b) == 0
来源：http://aks.jyoumei.cn

[S07] C：数组遍历求和
来源：http://qek.aizwys.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ruo.smart0.xyz

[S08] C：动态内存分配与释放
来源：http://osx.ydzc1.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lgz.wangdashe.top

[S09] C：结构体定义与初始化
来源：http://akc.shanyushiyangtech.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mtr.havefunace.top

[S10] C：指针与解引用
来源：http://siz.aibaodan.cn

int *p = &a;  *p = 5;
来源：http://tlx.meibo888.top

[S11] C：逐行读文件
来源：http://eko.bjfxy.top

FILE *f = fopen("a.txt", "r");
来源：http://cjn.iojbl.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qrr.pengpengdd.cyou

fclose(f);
来源：http://uac.xziqi.cn

[S12] C：写文件
来源：http://lov.yfazqb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://otw.daria6918.cn

[S13] C：宏定义
来源：http://zjx.ivvv.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://foq.jinqigfzy.top

[S14] C：枚举
来源：http://voi.yj20258888.top

enum Color { RED, GREEN, BLUE };
来源：http://xsf.yvedp.cn

[S15] C：类型转换
来源：http://emj.birdmap.top

(double) a / b
来源：http://qip.dashuyun.cn

[S16] C：位操作置位
来源：http://eoz.kuanghao11.cn

x |= (1 << 3);
来源：http://cow.zhongyouzk.top

[S17] C：安全拼接字符串
来源：http://osx.jiagoushi.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://efs.kuanghao11.cn

[S18] C：命令行参数
来源：http://vrp.gaohongyu789.top

int main(int argc, char **argv)
来源：http://ixt.nanxinkj.top

[S19] C：快速排序
来源：http://pme.jqgfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://bon.feifeiyinyue.top

[S20] C：二分查找
来源：http://pnz.jinyuanbaomall.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ukp.zdbjq.cn

[S21] C：字符类别判断
来源：http://uit.fengsongda.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bcj.zdqjudy.top

[S22] C：字符串转数字
来源：http://wsf.tarul.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jig.yuanzhike.top

[S23] C：随机数
来源：http://eds.bjfxy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://cqv.sufxvd.cn

[S24] C：获取本地时间
来源：http://zdg.hnqzz.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kka.dashuyun.cn

[S25] C：内存拷贝
来源：http://joi.kuanghao11.cn

memcpy(dst, src, n);
来源：http://brf.shanyushiyangkeji.top

[S26] C：内存清零
来源：http://uqm.fengsongda.top

memset(a, 0, sizeof a);
来源：http://ktk.zhoulong.xyz

[S27] C：定义常量
来源：http://vxq.kuanghao11.cn

const double PI = 3.14159;
来源：http://qmn.hesvh.cn

[S28] C：静态变量
来源：http://mcn.cucudq.cn

static int counter = 0;
来源：http://ant.c1oappe.top

[S29] C：变参函数
来源：http://zgo.zdqjudy.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://npc.cdnleiting.top

[S30] C：头文件保护
来源：http://qic.yj202588.top

#ifndef X_H
来源：http://tlp.chenjidiqi.icu

#define X_H
来源：http://yzd.shanyushiyangkeji.top

#endif
来源：http://vmu.pengpengdd.cyou

[S31] C++：Hello World
来源：http://pjg.jqgfzy.top

#include <iostream>
来源：http://apm.jiagoushi.top

int main() { std::cout << "Hello\n"; }
来源：http://aoa.ydzc1.top

[S32] C++：字符串
来源：http://mqn.zdbjq.cn

std::string s = "hi";  s += "!";
来源：http://wnr.zhixingplan.top

[S33] C++：vector 增删
来源：http://cvj.dianchejie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://czi.hammf.cn

[S34] C++：遍历 vector
来源：http://yex.bjfxy.top

for (auto &x : v) { std::cout << x; }
来源：http://tkm.cashguo.top

[S35] C++：map
来源：http://jaa.shanyushiyangtech.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ski.aibaodan.cn

[S36] C++：unordered_map
来源：http://vce.cqqwz.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uns.zhongyouzk.top

[S37] C++：set
来源：http://leh.jqgfzy.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nzu.zhaomingkeji.xyz

[S38] C++：排序
来源：http://ukb.jinqigufen.top

std::sort(v.begin(), v.end());
来源：http://zuh.hnxiangtu.top

[S39] C++：自定义比较器排序
来源：http://zxs.hongshengwenyu.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://csv.gaohongyu789.top

[S40] C++：查找元素
来源：http://lii.chenjidiqi.icu

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ukl.wangshuangyany.cn

[S41] C++：类与构造函数
来源：http://sse.bjfxy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tjj.yanxiufei.cn

[S42] C++：继承与虚函数
来源：http://hly.gzhubu.top

class B : public Base { public: void f() override {} };
来源：http://nuu.0kj1m.cn

[S43] C++：智能指针
来源：http://qxy.nanxinkj.top

auto p = std::make_unique<int>(5);
来源：http://anu.gotoacloud.top

[S44] C++：引用传参
来源：http://yjl.xziqi.cn

void inc(int &x) { ++x; }
来源：http://vcg.hongshengwenyu.top

[S45] C++：lambda
来源：http://jqs.fanxiaobao.xyz

auto add = [](int a, int b) { return a + b; };
来源：http://fev.zdqjudy.top

[S46] C++：函数模板
来源：http://hks.hywenlv.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://okv.nanxinkj.top

[S47] C++：结构化绑定遍历
来源：http://gey.kuanghao11.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vbo.ehwqpu.com

[S48] C++：逐行读文件
来源：http://aos.ppjwa.cn

std::ifstream in("a.txt");  std::string line;
来源：http://amr.xingfuxueyuan.xyz

while (std::getline(in, line)) { }
来源：http://rkb.dianchejie.cn

[S49] C++：写文件
来源：http://yzh.zhengqikj.top

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fzl.sxryk.cn

[S50] C++：格式化数字
来源：http://jip.yuanzhike.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fah.jqgfzy.top

[S51] C++：显式类型转换
来源：http://lbl.ehwqpu.com

static_cast<double>(a) / b
来源：http://oqi.ppjwa.cn

[S52] C++：const 与 noexcept
来源：http://ynn.snrcjt.cn

int size() const noexcept { return n_; }
来源：http://sph.hnxiangtu.top

[S53] C++：移动语义
来源：http://gvq.fanxiaobao.xyz

std::vector<int> w = std::move(v);
来源：http://ewt.bjfxy.top

[S54] C++：异常处理
来源：http://atw.snrcjt.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qfp.chenlongwang.top

[S55] C++：结构化绑定
来源：http://ixu.cashguo.top

auto [a, b] = std::make_pair(1, 2);
来源：http://lei.316326.xyz

[S56] C++：optional
来源：http://ysu.9152youxi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://glp.shanyushiyangkeji.top

[S57] C++：编译期常量
来源：http://vbm.xinyue.icu

constexpr int N = 10;
来源：http://jct.zhiwuduotai.top

[S58] C++：命名空间
来源：http://ooj.dashuyun.cn

namespace ns { int f() { return 1; } }
来源：http://dmj.birdmap.top

[S59] C++：静态断言
来源：http://yhh.xziqi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qes.fktsv.cn

[S60] C++：遍历并删除元素
来源：http://acd.yangfankeji.com


<!-- 参考信息 -->