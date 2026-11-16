代发 wailian999

[Q86] 读取 JSON 字段
来源：http://ade.uphjek.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://qin.yuxming.cn

[Q87] JSON 字段做条件
来源：http://znq.yangfankeji.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://tzc.shzxlz.cn

[Q88] 行转列（条件聚合）
来源：http://wnk.shzxlz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oxa.meibo888.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xiq.jinqigfzy.top

[Q89] 判断表是否存在
来源：http://gbk.cqqwz.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://loh.shuidangran.top

[Q90] 生成序号列
来源：http://vvi.jqgufenzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xbk.nanxuanxn.top

================================================================================
来源：http://jud.yj20258.top

R. Bash 专题
来源：http://msp.zhaomingkeji.xyz

================================================================================
来源：http://sag.meibo888.top

[R01] shebang 与严格模式
来源：http://tzk.hesvh.cn

#!/usr/bin/env bash
来源：http://psy.jinqigufen.top

set -euo pipefail
来源：http://uqq.birdmap.top

[R02] 变量赋值与使用
来源：http://ykh.zdbjq.cn

name="Tom"; echo "$name"
来源：http://rof.yanxiufei.cn

[R03] 只读变量
来源：http://ejt.cheryme.top

readonly PI=3.14
来源：http://oyp.cashguo.top

[R04] 位置参数
来源：http://imz.hesvh.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nmq.nwbrower.top

[R05] 参数默认值
来源：http://lid.tarul.cn

name="${1:-default}"
来源：http://tbj.bjfxy.top

[R06] 判断命令是否存在
来源：http://amv.xziqi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://eab.nwbrower.top

[R07] if 判断文件
来源：http://zbg.kuanghao11.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dsr.cqqwz.cn

[R08] 数值比较
来源：http://koe.shanyushiyangtech.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tpn.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://jiz.yangfankeji.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qoe.zhoulong.xyz

[R10] 正则匹配
来源：http://vud.cheryme.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://avc.yanxiufei.cn

[R11] case 多分支
来源：http://qgd.haohaochexian.top

case "$1" in
来源：http://xer.birdmap.top

start) echo "启动" ;;
来源：http://gwj.jinqigufen.top

stop)  echo "停止" ;;
来源：http://fvo.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://wbf.yanxiufei.cn

esac
来源：http://egx.hammf.cn

[R12] for 遍历文件
来源：http://pyp.hysaishi.cn

for f in *.txt; do echo "$f"; done
来源：http://git.sufxvd.cn

[R13] for 计数循环
来源：http://hda.gzhubu.top

for i in {1..10}; do echo "$i"; done
来源：http://rkx.hesvh.cn

[R14] C 风格 for
来源：http://nui.xuetiantiany.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xlr.aibaodan.cn

[R15] while 逐行读文件
来源：http://hla.uphjek.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fzq.tianlin.xyz

[R16] until 等待条件
来源：http://xnd.kuanghao11.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iim.316326.xyz

[R17] 数组定义与取值
来源：http://cfk.sufxvd.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ezr.chenjidiqi.icu

[R18] 遍历数组
来源：http://oaq.52xcode.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mfr.bjfxy.top

[R19] 数组长度
来源：http://esh.jinqigufen.top

echo "${#arr[@]}"
来源：http://krn.ppjwa.cn

[R20] 关联数组（字典）
来源：http://wfb.hywenlv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ewz.yuxming.cn

[R21] 字符串长度
来源：http://wsp.kuanghao11.cn

echo "${#s}"
来源：http://doh.fktsv.cn

[R22] 截取子串
来源：http://for.chenlongwang.top

echo "${s:0:5}"
来源：http://hov.jqgfzy.top

[R23] 字符串替换
来源：http://fls.vehdjk.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://yox.ppjwa.cn

[R24] 大小写转换
来源：http://tya.haohaochexian.top

echo "${s^^}"; echo "${s,,}"
来源：http://nhz.hywenlv.cn

[R25] 去后缀 / 去前缀
来源：http://bvc.tarul.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://aqz.xziqi.cn

[R26] 命令替换
来源：http://gwi.cheryme.top

now=$(date +%F); echo "$now"
来源：http://wda.cqqwz.cn

[R27] 算术展开
来源：http://nvd.yanxiufei.cn

echo $((1 + 2 * 3))
来源：http://wzg.zycfv.cn

[R28] 浮点运算
来源：http://lgs.zhijiandao.cn

echo "scale=2; 10/3" | bc
来源：http://ctc.9152youxi.cn

[R29] 定义函数
来源：http://asi.zdbjq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ejm.daxiang520.top

[R30] 函数返回状态码
来源：http://xee.yangfankeji.com

f() { return 0; }; f || echo "失败了"
来源：http://tdp.yongpay.top

[R31] 局部变量
来源：http://tis.fanxiaobao.xyz

f() { local x=1; echo "$x"; }
来源：http://vsy.gzhubu.top

[R32] 参数个数校验
来源：http://xkl.nanxinkj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yxi.yonumen.top

[R33] 捕获错误并提示行号
来源：http://lkt.zhijiandao.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jpj.316326.xyz

[R34] 退出时清理
来源：http://dmb.daxiang520.top

trap 'rm -f "$tmp"' EXIT
来源：http://dbg.sweek.top

[R35] 后台执行并等待
来源：http://wum.jinyuanbaomall.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fpt.hywenlv.cn

[R36] 并发执行多个任务
来源：http://zuj.cqqwz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ixr.cheryme.top

[R37] 把输出赋给变量
来源：http://qib.zhoulong.xyz

files=$(ls -1)
来源：http://ymc.sxryk.cn

[R38] 管道串联
来源：http://nsr.jianghu66.top

cat a.txt | grep -i error | wc -l
来源：http://tyf.hesvh.cn

[R39] 重定向标准输出与错误
来源：http://fgu.0kj1m.cn

cmd > out.log 2>&1
来源：http://dop.shanyushiyangtech.top

[R40] 追加写日志
来源：http://aqx.birdmap.top

echo "log" >> out.log
来源：http://ows.cucudq.cn

[R41] 丢弃输出
来源：http://xsy.zhaomingkeji.xyz

cmd >/dev/null 2>&1
来源：http://wwz.daxiang520.top

[R42] 输入重定向
来源：http://jle.zhixingplan.top

wc -l < a.txt
来源：http://myo.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://zgj.ywan-chungtsiang.top

find . -name "*.log" -type f
来源：http://hon.andypj.xyz

[R44] 按修改时间查找
来源：http://vjh.yongpay.top

find . -mtime -7 -type f
来源：http://xjn.yj202588.top

[R45] 批量删除
来源：http://sxq.nanxuanxn.top

find . -name "*.tmp" -delete
来源：http://piv.fktsv.cn

[R46] 递归替换文件内容
来源：http://gpx.vehdjk.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rzw.cucudq.cn

[R47] sed 单行替换
来源：http://hgj.zhaomingkeji.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://lej.chenjidiqi.icu

[R48] awk 取指定列
来源：http://qwp.nwbrower.top

awk '{print $1, $3}' a.txt
来源：http://lxz.hfpthk.cn

[R49] awk 带条件
来源：http://rvr.guowangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ezv.smart0.xyz

[R50] awk 求和
来源：http://bgv.yvedp.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zbt.xingfuxueyuan.xyz

[R51] 排序去重取前几
来源：http://jfh.gzhubu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://xjt.chenzaomai.com

[R52] 统计行数
来源：http://tra.yanxiufei.cn

wc -l a.txt
来源：http://oeh.epnwcf.com

[R53] 查看文件头与实时尾
来源：http://nvd.cheryme.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rmu.yfazqb.com

[R54] 比较两个文件
来源：http://gky.jlsjyb.cn

diff a.txt b.txt
来源：http://zcf.chenlongwang.top

[R55] 压缩与解压
来源：http://hul.gogol.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rop.yangfankeji.com

[R56] 远程拷贝
来源：http://tsi.jqgfzy.top

scp file user@host:/path/
来源：http://ghs.yongpay.top

[R57] 远程执行命令
来源：http://amt.wangdashe.top

ssh user@host 'uptime'
来源：http://hld.guannengcc.top

[R58] 下载文件
来源：http://ogx.zdbjq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cwl.andypj.xyz

[R59] 发 POST JSON
来源：http://jrt.yfazqb.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nkf.chenlongwang.top

[R60] 只看 HTTP 状态码
来源：http://sjh.svipenyu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bsc.andypj.xyz

[R61] 磁盘占用
来源：http://hra.cqqwz.cn

df -h;  du -sh *
来源：http://nuo.jqgfzy.top

[R62] 找最占空间的文件
来源：http://sbi.vqdsnc.cn

du -ah . | sort -rh | head -10
来源：http://lmm.birdmap.top

[R63] 内存与进程
来源：http://ejo.hnxiangtu.top

free -h;  ps aux | grep nginx
来源：http://xvw.zhengqikj.top

[R64] 结束进程
来源：http://vqg.c1oappe.top

kill -9 $(pgrep -f app.py)
来源：http://amr.316326.xyz

[R65] 查看端口占用
来源：http://xix.gogol.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ehg.yanxiufei.cn

[R66] 定时任务
来源：http://msn.hcnkem.com

crontab -e;  crontab -l
来源：http://rdz.dashuyun.cn

[R67] 生成随机十六进制串
来源：http://eay.jlsjyb.cn

openssl rand -hex 16
来源：http://gdp.316326.xyz

[R68] 计算文件校验值
来源：http://tjf.gotoacloud.top

sha256sum a.txt;  md5sum a.txt
来源：http://pba.smart0.xyz

[R69] 生成随机密码
来源：http://kja.nanxinkj.top

head -c 16 /dev/urandom | base64
来源：http://ohe.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://dlo.birdmap.top

date +%s;  date -d @1700000000
来源：http://ben.vehdjk.com

[R71] 日期格式化
来源：http://rat.fktsv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nej.sweek.top

[R72] 等待端口就绪
来源：http://pnl.shanyushiyangtech.top

until nc -z localhost 3306; do sleep 1; done
来源：http://fzi.quarkkingdee.top

[R73] 分割大日志
来源：http://qdy.0kj1m.cn

split -l 1000 big.log part_
来源：http://ipt.yvedp.cn

[R74] 批量重命名
来源：http://lre.wangshuangyany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://uqz.hfpthk.cn

[R75] 导出环境变量
来源：http://rkj.birdmap.top

export PATH="$HOME/bin:$PATH"
来源：http://vqj.zhixingplan.top

[R76] 使用临时文件
来源：http://iqf.cdnleiting.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ejk.zdbjq.cn

[R77] 读取用户输入
来源：http://ycw.sxryk.cn

read -rp "请输入: " ans
来源：http://iwn.shuidangran.top

[R78] 交互式菜单
来源：http://qwa.hongshengwenyu.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wob.zycfv.cn

[R79] 解析命令行选项
来源：http://bfq.hfpthk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vwz.dianchejie.cn

[R80] 查看脚本执行耗时
来源：http://mie.dashuyun.cn

time ./run.sh
来源：http://nom.bjfxy.top

================================================================================
来源：http://zeb.jqgufenzy.top

S. C / C++ 专题
来源：http://mrj.jinqigfzy.top

================================================================================
来源：http://sev.fktsv.cn

[S01] C：Hello World
来源：http://dfp.xziqi.cn

#include <stdio.h>
来源：http://gjr.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zqb.shanyushiyangtech.top

[S02] C：变量与格式化输出
来源：http://nno.hongshengwenyu.top

int a = 10; printf("%d\n", a);
来源：http://myk.aizwys.cn

[S03] C：读入整数
来源：http://zdu.ctjpmb.com

int x; scanf("%d", &x);
来源：http://vud.gaohongyu789.top

[S04] C：字符串复制
来源：http://jzh.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://rkv.yj202588.top

[S05] C：字符串长度
来源：http://jdi.tanke756.top

strlen(s)
来源：http://vwk.ydjk.org.cn

[S06] C：字符串比较
来源：http://tse.hfpthk.cn

strcmp(a, b) == 0
来源：http://ryv.quarkkingdee.top

[S07] C：数组遍历求和
来源：http://poj.yuanzhike.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://nhq.zhoulong.xyz

[S08] C：动态内存分配与释放
来源：http://uji.yj20258888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iuc.jinqigfzy.top

[S09] C：结构体定义与初始化
来源：http://pqt.uphjek.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fcu.guannengcc.top

[S10] C：指针与解引用
来源：http://nmd.yj20258888.top

int *p = &a;  *p = 5;
来源：http://unt.ydzc1.top

[S11] C：逐行读文件
来源：http://fsc.jiagoushi.top

FILE *f = fopen("a.txt", "r");
来源：http://wuj.gotoacloud.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tfv.gzhubu.top

fclose(f);
来源：http://imr.jyoumei.cn

[S12] C：写文件
来源：http://fsi.wangshuangyany.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qtt.redwolf501.top

[S13] C：宏定义
来源：http://zyc.tanke756.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dcj.tarul.cn

[S14] C：枚举
来源：http://cpx.xingfuxueyuan.xyz

enum Color { RED, GREEN, BLUE };
来源：http://wtj.yvedp.cn

[S15] C：类型转换
来源：http://ngy.epnwcf.com

(double) a / b
来源：http://fie.vehdjk.com

[S16] C：位操作置位
来源：http://hgs.hesvh.cn

x |= (1 << 3);
来源：http://bzg.ydzc1.top

[S17] C：安全拼接字符串
来源：http://fvk.bbcook.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rkw.vqdsnc.cn

[S18] C：命令行参数
来源：http://ltx.zhijiandao.cn

int main(int argc, char **argv)
来源：http://mqf.meibo888.top

[S19] C：快速排序
来源：http://rsx.guannengcc.top

qsort(a, n, sizeof(int), cmp);
来源：http://nxs.sufxvd.cn

[S20] C：二分查找
来源：http://kqn.zhongyouzk.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://uzi.tian-w.cn

[S21] C：字符类别判断
来源：http://bmm.zdqjudy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pdl.nanxinkj.top

[S22] C：字符串转数字
来源：http://war.chenjidiqi.icu

atoi("42");  strtod("3.14", NULL);
来源：http://kut.jinqigufen.top

[S23] C：随机数
来源：http://jfj.hfpthk.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vgu.fzhhl.top

[S24] C：获取本地时间
来源：http://ipr.birdmap.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://shd.sufxvd.cn

[S25] C：内存拷贝
来源：http://sqp.xuanzx.com

memcpy(dst, src, n);
来源：http://sth.haohaochexian.top

[S26] C：内存清零
来源：http://sey.cqqwz.cn

memset(a, 0, sizeof a);
来源：http://tlj.yueranfly.top

[S27] C：定义常量
来源：http://ufs.hnqzz.top

const double PI = 3.14159;
来源：http://olj.52xcode.cn

[S28] C：静态变量
来源：http://njr.jyoumei.cn

static int counter = 0;
来源：http://nnh.yonumen.top

[S29] C：变参函数
来源：http://mpp.yj20258.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://thy.svipenyu.cn

[S30] C：头文件保护
来源：http://wnp.shangyingyoupin.top

#ifndef X_H
来源：http://ioe.jqgufenzy.top

#define X_H
来源：http://obx.snrcjt.cn

#endif
来源：http://jaw.yongpay.top

[S31] C++：Hello World
来源：http://dcu.pengpengdd.cyou

#include <iostream>
来源：http://qaf.gotoacloud.top

int main() { std::cout << "Hello\n"; }
来源：http://tnr.yj202588.top

[S32] C++：字符串
来源：http://iwc.jinqigfzy.top

std::string s = "hi";  s += "!";
来源：http://nax.hcnkem.com

[S33] C++：vector 增删
来源：http://wqp.xuetiantiany.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://szy.ehwqpu.com

[S34] C++：遍历 vector
来源：http://bbn.epnwcf.com

for (auto &x : v) { std::cout << x; }
来源：http://fnl.hysaishi.cn

[S35] C++：map
来源：http://gkk.zhongyouzk.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hju.daxiang520.top

[S36] C++：unordered_map
来源：http://klu.cdnleiting.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://del.dianchejie.cn

[S37] C++：set
来源：http://bbu.shzxlz.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ncg.xuetiantiany.cn

[S38] C++：排序
来源：http://uej.hongshengwenyu.top

std::sort(v.begin(), v.end());
来源：http://xah.cheryme.top

[S39] C++：自定义比较器排序
来源：http://nlf.pengpengdd.cyou

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cca.tarul.cn

[S40] C++：查找元素
来源：http://ftn.quarkkingdee.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://dvu.hysaishi.cn

[S41] C++：类与构造函数
来源：http://zob.jiagoushi.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://aoa.jinqigfzy.top

[S42] C++：继承与虚函数
来源：http://egx.sjlbkw.cn

class B : public Base { public: void f() override {} };
来源：http://gux.ppjwa.cn

[S43] C++：智能指针
来源：http://eoo.xuetiantiany.cn

auto p = std::make_unique<int>(5);
来源：http://oxb.fengsongda.top

[S44] C++：引用传参
来源：http://xdy.andypj.xyz

void inc(int &x) { ++x; }
来源：http://szv.nwbrower.top

[S45] C++：lambda
来源：http://aen.cheryme.top

auto add = [](int a, int b) { return a + b; };
来源：http://qjs.pycfn.com

[S46] C++：函数模板
来源：http://wrz.pengpengdd.cyou

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tgx.havefunace.top

[S47] C++：结构化绑定遍历
来源：http://aop.fengsongda.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nig.iojbl.cn

[S48] C++：逐行读文件
来源：http://dyh.cqqwz.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lyf.mhx1999.top

while (std::getline(in, line)) { }
来源：http://wmu.yfazqb.com

[S49] C++：写文件
来源：http://koa.jinyuanbaomall.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sen.52xcode.cn

[S50] C++：格式化数字
来源：http://ibx.jyoumei.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pbh.feifeiyinyue.top

[S51] C++：显式类型转换
来源：http://ryl.hcnkem.com

static_cast<double>(a) / b
来源：http://gjq.nanxinkj.top

[S52] C++：const 与 noexcept
来源：http://imk.nwbrower.top

int size() const noexcept { return n_; }
来源：http://mmk.pengpengdd.cyou

[S53] C++：移动语义
来源：http://kiy.hcnkem.com

std::vector<int> w = std::move(v);
来源：http://rog.yvedp.cn

[S54] C++：异常处理
来源：http://vzi.zhengqikj.top

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gke.yj202588.top

[S55] C++：结构化绑定
来源：http://lra.yvedp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wro.chenlongwang.top

[S56] C++：optional
来源：http://zrc.yongpay.top


<!-- 参考信息 -->