代发 wailian999

[Q82] 字符长度与字节长度
来源：http://ald.shuidangran.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yse.dashuyun.cn

[Q83] 大小写转换
来源：http://jkt.ywan-chungtsiang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://htk.zhoulong.xyz

[Q84] 去除首尾空格
来源：http://ilj.zhongyouzk.top

SELECT TRIM(name) FROM users;
来源：http://qir.svipenyu.cn

[Q85] 数值取整
来源：http://vbr.pycfn.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vxg.guannengcc.top

[Q86] 读取 JSON 字段
来源：http://wmw.cheryme.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nks.zhaomingkeji.xyz

[Q87] JSON 字段做条件
来源：http://yfr.yj202588.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vra.bjfxy.top

[Q88] 行转列（条件聚合）
来源：http://hog.yongpay.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fzc.xziqi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zdv.gogol.net.cn

[Q89] 判断表是否存在
来源：http://yxv.hnqzz.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://sqb.jqgufenzy.top

[Q90] 生成序号列
来源：http://poe.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://vey.meibo888.top

================================================================================
来源：http://hlf.chenlongwang.top

R. Bash 专题
来源：http://wcq.ehwqpu.com

================================================================================
来源：http://kui.yfazqb.com

[R01] shebang 与严格模式
来源：http://rbu.snrcjt.cn

#!/usr/bin/env bash
来源：http://ime.nanxinkj.top

set -euo pipefail
来源：http://qlu.jinqigfzy.top

[R02] 变量赋值与使用
来源：http://zsy.zhijiandao.cn

name="Tom"; echo "$name"
来源：http://zzn.yuanzhike.top

[R03] 只读变量
来源：http://rnj.epnwcf.com

readonly PI=3.14
来源：http://btm.meibo888.top

[R04] 位置参数
来源：http://cdi.hywenlv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vqv.cheryme.top

[R05] 参数默认值
来源：http://pnl.redwolf501.top

name="${1:-default}"
来源：http://vvs.zhongyouzk.top

[R06] 判断命令是否存在
来源：http://opp.birdmap.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://xbg.shanyushiyangtech.top

[R07] if 判断文件
来源：http://cnz.dashuyun.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hik.dashuyun.cn

[R08] 数值比较
来源：http://gvn.ppjwa.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lkp.jianghu66.top

[R09] 字符串比较
来源：http://vir.zhixingplan.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gws.havefunace.top

[R10] 正则匹配
来源：http://zgb.gzhubu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hjv.fengsongda.top

[R11] case 多分支
来源：http://wxx.shangyingyoupin.top

case "$1" in
来源：http://yng.yongpay.top

start) echo "启动" ;;
来源：http://nlo.cucudq.cn

stop)  echo "停止" ;;
来源：http://hos.nwbrower.top

*)     echo "未知命令" ;;
来源：http://bdz.smart0.xyz

esac
来源：http://uhj.havefunace.top

[R12] for 遍历文件
来源：http://aow.sxryk.cn

for f in *.txt; do echo "$f"; done
来源：http://hcb.dianchejie.cn

[R13] for 计数循环
来源：http://tpy.yfazqb.com

for i in {1..10}; do echo "$i"; done
来源：http://kjq.nanxinkj.top

[R14] C 风格 for
来源：http://yew.mhx1999.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uqs.yangfankeji.com

[R15] while 逐行读文件
来源：http://nqz.svipenyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jmm.fengsongda.top

[R16] until 等待条件
来源：http://qnp.jinqigfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://znh.pycfn.com

[R17] 数组定义与取值
来源：http://smz.ctjpmb.com

arr=(a b c); echo "${arr[0]}"
来源：http://jrr.epnwcf.com

[R18] 遍历数组
来源：http://auh.9152youxi.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qwo.52xcode.cn

[R19] 数组长度
来源：http://zhb.yj20258.top

echo "${#arr[@]}"
来源：http://qki.hfpthk.cn

[R20] 关联数组（字典）
来源：http://kqu.ydjk.org.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xvr.chenjidiqi.icu

[R21] 字符串长度
来源：http://wya.9152youxi.cn

echo "${#s}"
来源：http://ecc.dashuyun.cn

[R22] 截取子串
来源：http://agt.gzhubu.top

echo "${s:0:5}"
来源：http://ohw.jinghuilouyu.cn

[R23] 字符串替换
来源：http://odd.wangshuangyany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://phg.pengpengdd.cyou

[R24] 大小写转换
来源：http://eyu.ywan-chungtsiang.top

echo "${s^^}"; echo "${s,,}"
来源：http://xwg.yj202588.top

[R25] 去后缀 / 去前缀
来源：http://gcp.cucudq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://xxj.ybcxt.top

[R26] 命令替换
来源：http://aed.bjfxy.top

now=$(date +%F); echo "$now"
来源：http://sau.yuxming.cn

[R27] 算术展开
来源：http://nuj.nwbrower.top

echo $((1 + 2 * 3))
来源：http://iml.zhongyouzk.top

[R28] 浮点运算
来源：http://xgf.cdnleiting.top

echo "scale=2; 10/3" | bc
来源：http://vrn.gogol.net.cn

[R29] 定义函数
来源：http://nrh.fanxiaobao.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://eyc.hnqzz.top

[R30] 函数返回状态码
来源：http://eds.pengpengdd.cyou

f() { return 0; }; f || echo "失败了"
来源：http://iog.sysykeji.top

[R31] 局部变量
来源：http://lvf.yfazqb.com

f() { local x=1; echo "$x"; }
来源：http://lvh.yangfankeji.com

[R32] 参数个数校验
来源：http://lcy.aizwys.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tio.c1oappe.top

[R33] 捕获错误并提示行号
来源：http://kzf.hysaishi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mie.ctjpmb.com

[R34] 退出时清理
来源：http://sma.hammf.cn

trap 'rm -f "$tmp"' EXIT
来源：http://voa.shanyushiyangkeji.top

[R35] 后台执行并等待
来源：http://dsf.zycfv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://sqy.jqgfzy.top

[R36] 并发执行多个任务
来源：http://qku.cashguo.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://dyi.sjlbkw.cn

[R37] 把输出赋给变量
来源：http://rdm.birdmap.top

files=$(ls -1)
来源：http://icr.chenzaomai.com

[R38] 管道串联
来源：http://hwr.hnqzz.top

cat a.txt | grep -i error | wc -l
来源：http://gou.ywan-chungtsiang.top

[R39] 重定向标准输出与错误
来源：http://eja.haohaochexian.top

cmd > out.log 2>&1
来源：http://jfg.hammf.cn

[R40] 追加写日志
来源：http://dqq.dianchejie.cn

echo "log" >> out.log
来源：http://sgk.cucudq.cn

[R41] 丢弃输出
来源：http://awx.vqdsnc.cn

cmd >/dev/null 2>&1
来源：http://fat.jianghu66.top

[R42] 输入重定向
来源：http://xzu.nanxinkj.top

wc -l < a.txt
来源：http://cfi.ybcxt.top

[R43] 按名字查找文件
来源：http://wao.yj20258.top

find . -name "*.log" -type f
来源：http://pdl.hcnkem.com

[R44] 按修改时间查找
来源：http://ejd.hcnkem.com

find . -mtime -7 -type f
来源：http://dcs.yongpay.top

[R45] 批量删除
来源：http://jtv.nwbrower.top

find . -name "*.tmp" -delete
来源：http://xvg.xingfuxueyuan.xyz

[R46] 递归替换文件内容
来源：http://fup.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://iyf.hesvh.cn

[R47] sed 单行替换
来源：http://kdx.hesvh.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hpx.uphjek.com

[R48] awk 取指定列
来源：http://qys.xinyue.icu

awk '{print $1, $3}' a.txt
来源：http://qsx.tanke756.top

[R49] awk 带条件
来源：http://tpy.shuidangran.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wxo.yongpay.top

[R50] awk 求和
来源：http://kru.shanyushiyangtech.top

awk '{s += $2} END {print s}' a.txt
来源：http://oql.vqdsnc.cn

[R51] 排序去重取前几
来源：http://kdy.birdmap.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gnl.hysaishi.cn

[R52] 统计行数
来源：http://grt.yueranfly.top

wc -l a.txt
来源：http://vxt.aibaodan.cn

[R53] 查看文件头与实时尾
来源：http://qep.smart0.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wtx.hysaishi.cn

[R54] 比较两个文件
来源：http://hml.ydzc1.top

diff a.txt b.txt
来源：http://yjs.aibaodan.cn

[R55] 压缩与解压
来源：http://xdk.jlsjyb.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ykm.tarul.cn

[R56] 远程拷贝
来源：http://zau.shanyushiyangtech.top

scp file user@host:/path/
来源：http://fom.havefunace.top

[R57] 远程执行命令
来源：http://vvo.zycfv.cn

ssh user@host 'uptime'
来源：http://mbv.guowangkeji.top

[R58] 下载文件
来源：http://gqb.wangdashe.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qbk.zycfv.cn

[R59] 发 POST JSON
来源：http://rtq.daria6918.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://twr.svipenyu.cn

[R60] 只看 HTTP 状态码
来源：http://oyk.dianchejie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://drt.bjfxy.top

[R61] 磁盘占用
来源：http://msk.redwolf501.top

df -h;  du -sh *
来源：http://yzf.ctjpmb.com

[R62] 找最占空间的文件
来源：http://vpj.hywenlv.cn

du -ah . | sort -rh | head -10
来源：http://cfs.zhixingplan.top

[R63] 内存与进程
来源：http://wqc.nanxuanxn.top

free -h;  ps aux | grep nginx
来源：http://dyr.fengsongda.top

[R64] 结束进程
来源：http://pgs.jianghu66.top

kill -9 $(pgrep -f app.py)
来源：http://azc.xziqi.cn

[R65] 查看端口占用
来源：http://vqi.vqdsnc.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kzi.fengsongda.top

[R66] 定时任务
来源：http://jqf.jinqigufen.top

crontab -e;  crontab -l
来源：http://lda.tarul.cn

[R67] 生成随机十六进制串
来源：http://xfg.fzhhl.top

openssl rand -hex 16
来源：http://liv.havefunace.top

[R68] 计算文件校验值
来源：http://qhq.hfpthk.cn

sha256sum a.txt;  md5sum a.txt
来源：http://enk.hnqzz.top

[R69] 生成随机密码
来源：http://omy.meibo888.top

head -c 16 /dev/urandom | base64
来源：http://dmu.sjlbkw.cn

[R70] 时间戳与互转
来源：http://slj.shanyushiyangtech.top

date +%s;  date -d @1700000000
来源：http://aqn.yj202588.top

[R71] 日期格式化
来源：http://rvf.pycfn.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://lfx.zhoulong.xyz

[R72] 等待端口就绪
来源：http://qgc.pengpengdd.cyou

until nc -z localhost 3306; do sleep 1; done
来源：http://iyb.jianghu66.top

[R73] 分割大日志
来源：http://trv.jiagoushi.top

split -l 1000 big.log part_
来源：http://wbs.hnxiangtu.top

[R74] 批量重命名
来源：http://gnz.smart0.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kxb.chenjidiqi.icu

[R75] 导出环境变量
来源：http://vaj.kuanghao11.cn

export PATH="$HOME/bin:$PATH"
来源：http://wkw.0kj1m.cn

[R76] 使用临时文件
来源：http://rlt.zhaomingkeji.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oul.redwolf501.top

[R77] 读取用户输入
来源：http://nnp.zhijiandao.cn

read -rp "请输入: " ans
来源：http://pka.fanxiaobao.xyz

[R78] 交互式菜单
来源：http://pjv.fzhhl.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rfs.ctjpmb.com

[R79] 解析命令行选项
来源：http://lye.shzxlz.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nuw.bbcook.cn

[R80] 查看脚本执行耗时
来源：http://vjn.zycfv.cn

time ./run.sh
来源：http://evu.ivvv.top

================================================================================
来源：http://vrc.andypj.xyz

S. C / C++ 专题
来源：http://kvi.shanyushiyangkeji.top

================================================================================
来源：http://fzt.yuxming.cn

[S01] C：Hello World
来源：http://hmo.tanke756.top

#include <stdio.h>
来源：http://ywa.vehdjk.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://hgd.birdmap.top

[S02] C：变量与格式化输出
来源：http://xtp.jinghuilouyu.cn

int a = 10; printf("%d\n", a);
来源：http://lnl.daria6918.cn

[S03] C：读入整数
来源：http://yoi.snrcjt.cn

int x; scanf("%d", &x);
来源：http://ntj.mhx1999.top

[S04] C：字符串复制
来源：http://hfx.shanyushiyangtech.top

char dst[32]; strcpy(dst, "hi");
来源：http://ghh.gaohongyu789.top

[S05] C：字符串长度
来源：http://zzl.tianlin.xyz

strlen(s)
来源：http://her.wangshuangyany.cn

[S06] C：字符串比较
来源：http://qyv.nwbrower.top

strcmp(a, b) == 0
来源：http://lul.ywan-chungtsiang.top

[S07] C：数组遍历求和
来源：http://wog.bbcook.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gte.ppjwa.cn

[S08] C：动态内存分配与释放
来源：http://qjy.birdmap.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mkv.ehwqpu.com

[S09] C：结构体定义与初始化
来源：http://hdd.cashguo.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aps.smart0.xyz

[S10] C：指针与解引用
来源：http://unw.ywan-chungtsiang.top

int *p = &a;  *p = 5;
来源：http://khe.uphjek.com

[S11] C：逐行读文件
来源：http://tui.xingfuxueyuan.xyz

FILE *f = fopen("a.txt", "r");
来源：http://rey.gotoacloud.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xkn.jiagoushi.top

fclose(f);
来源：http://wnu.gzhubu.top

[S12] C：写文件
来源：http://gzm.yfazqb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qbz.mhx1999.top

[S13] C：宏定义
来源：http://vuw.jinghuilouyu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jyy.xingfuxueyuan.xyz

[S14] C：枚举
来源：http://zzk.hnxiangtu.top

enum Color { RED, GREEN, BLUE };
来源：http://qua.xinyue.icu

[S15] C：类型转换
来源：http://gvf.ydzc1.top

(double) a / b
来源：http://qmv.mhx1999.top

[S16] C：位操作置位
来源：http://wgk.hongshengwenyu.top

x |= (1 << 3);
来源：http://jxj.bjfxy.top

[S17] C：安全拼接字符串
来源：http://xup.yonumen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lqs.ydjk.org.cn

[S18] C：命令行参数
来源：http://usm.redwolf501.top

int main(int argc, char **argv)
来源：http://aov.chenlongwang.top

[S19] C：快速排序
来源：http://oef.gzhubu.top

qsort(a, n, sizeof(int), cmp);
来源：http://xcj.epnwcf.com

[S20] C：二分查找
来源：http://vsf.xinyue.icu

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qri.haohaochexian.top

[S21] C：字符类别判断
来源：http://tcw.hfpthk.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ful.tarul.cn

[S22] C：字符串转数字
来源：http://ozm.sjlbkw.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xxq.sweek.top

[S23] C：随机数
来源：http://ujc.ywan-chungtsiang.top

srand(time(NULL));  int r = rand() % 100;
来源：http://wxp.yuanzhike.top

[S24] C：获取本地时间
来源：http://guw.c1oappe.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wbo.fehbvm.com

[S25] C：内存拷贝
来源：http://xza.ehwqpu.com

memcpy(dst, src, n);
来源：http://yqi.ydjk.org.cn

[S26] C：内存清零
来源：http://pyr.nanxinkj.top

memset(a, 0, sizeof a);
来源：http://jsq.yj202588.top

[S27] C：定义常量
来源：http://vik.andypj.xyz

const double PI = 3.14159;
来源：http://mps.xuanzx.com

[S28] C：静态变量
来源：http://vti.pengpengdd.cyou

static int counter = 0;
来源：http://eua.chenzaomai.com

[S29] C：变参函数
来源：http://glm.redwolf501.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qyu.ywan-chungtsiang.top

[S30] C：头文件保护
来源：http://ndl.gogol.net.cn

#ifndef X_H
来源：http://arv.ppjwa.cn

#define X_H
来源：http://srz.xingfuxueyuan.xyz

#endif
来源：http://mkp.chenzaomai.com

[S31] C++：Hello World
来源：http://wqa.jinqigufen.top

#include <iostream>
来源：http://mgm.tianlin.xyz

int main() { std::cout << "Hello\n"; }
来源：http://rrx.bjfxy.top

[S32] C++：字符串
来源：http://mji.wangdashe.top

std::string s = "hi";  s += "!";
来源：http://xqm.jiagoushi.top

[S33] C++：vector 增删
来源：http://glk.hfpthk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pyb.shzxlz.cn

[S34] C++：遍历 vector
来源：http://uex.ivvv.top

for (auto &x : v) { std::cout << x; }
来源：http://xgt.fehbvm.com

[S35] C++：map
来源：http://pxm.meibo888.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tvv.zhijiandao.cn

[S36] C++：unordered_map
来源：http://dau.316326.xyz

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cvr.hfpthk.cn

[S37] C++：set
来源：http://ngi.jianghu66.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hrv.pengpengdd.cyou

[S38] C++：排序
来源：http://gok.tian-w.cn

std::sort(v.begin(), v.end());
来源：http://lqn.wangdashe.top

[S39] C++：自定义比较器排序
来源：http://azc.jinqigfzy.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rcs.daria6918.cn

[S40] C++：查找元素
来源：http://wuo.cucudq.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pyv.snrcjt.cn

[S41] C++：类与构造函数
来源：http://hlr.birdmap.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hbo.jiagoushi.top

[S42] C++：继承与虚函数
来源：http://wsw.dianchejie.cn

class B : public Base { public: void f() override {} };
来源：http://avh.jinqigufen.top

[S43] C++：智能指针
来源：http://gls.jqgfzy.top

auto p = std::make_unique<int>(5);
来源：http://qby.cucudq.cn

[S44] C++：引用传参
来源：http://rde.gaohongyu789.top

void inc(int &x) { ++x; }
来源：http://idp.ehwqpu.com

[S45] C++：lambda
来源：http://qbl.birdmap.top

auto add = [](int a, int b) { return a + b; };
来源：http://lio.quarkkingdee.top

[S46] C++：函数模板
来源：http://wrl.52xcode.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mge.jlsjyb.cn

[S47] C++：结构化绑定遍历
来源：http://uqd.jqgfzy.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mwf.zdbjq.cn

[S48] C++：逐行读文件
来源：http://nni.sufxvd.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xxx.fzhhl.top

while (std::getline(in, line)) { }
来源：http://eri.xuetiantiany.cn

[S49] C++：写文件
来源：http://acv.hammf.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vna.sufxvd.cn

[S50] C++：格式化数字
来源：http://qzg.aibaodan.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dbo.yanxiufei.cn

[S51] C++：显式类型转换
来源：http://tjz.nwbrower.top

static_cast<double>(a) / b
来源：http://qsu.ybcxt.top

[S52] C++：const 与 noexcept
来源：http://ysg.tianlin.xyz


<!-- 参考信息 -->