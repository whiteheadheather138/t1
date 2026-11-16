代发 wailian999

[Q82] 字符长度与字节长度
来源：http://gaz.zhongyouzk.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xwt.zdqjudy.top

[Q83] 大小写转换
来源：http://mpd.xuetiantiany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hce.jinghuilouyu.cn

[Q84] 去除首尾空格
来源：http://sgu.yueranfly.top

SELECT TRIM(name) FROM users;
来源：http://bpb.zhengqikj.top

[Q85] 数值取整
来源：http://fgw.zhaomingkeji.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://aqq.jinghuilouyu.cn

[Q86] 读取 JSON 字段
来源：http://jpz.fengsongda.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://gay.jinyuanbaomall.cn

[Q87] JSON 字段做条件
来源：http://png.snrcjt.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uzl.ctjpmb.com

[Q88] 行转列（条件聚合）
来源：http://egn.sweek.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zvf.cashguo.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://lam.guowangkeji.top

[Q89] 判断表是否存在
来源：http://mco.smart0.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://akv.pycfn.com

[Q90] 生成序号列
来源：http://fqq.nwbrower.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hea.316326.xyz

================================================================================
来源：http://cfw.zhiwuduotai.top

R. Bash 专题
来源：http://gpj.yueranfly.top

================================================================================
来源：http://azo.zhiwuduotai.top

[R01] shebang 与严格模式
来源：http://sfk.jyoumei.cn

#!/usr/bin/env bash
来源：http://lef.gaohongyu789.top

set -euo pipefail
来源：http://bcr.hysaishi.cn

[R02] 变量赋值与使用
来源：http://ibh.zhengqikj.top

name="Tom"; echo "$name"
来源：http://vgj.tianlin.xyz

[R03] 只读变量
来源：http://eeg.hywenlv.cn

readonly PI=3.14
来源：http://gwg.birdmap.top

[R04] 位置参数
来源：http://lyq.xingfuxueyuan.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nan.bbcook.cn

[R05] 参数默认值
来源：http://jun.smart0.xyz

name="${1:-default}"
来源：http://jbh.uphjek.com

[R06] 判断命令是否存在
来源：http://vhr.aizwys.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://inf.yonumen.top

[R07] if 判断文件
来源：http://you.xuanzx.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://yex.tianlin.xyz

[R08] 数值比较
来源：http://sew.jiagoushi.top

if (( a > b )); then echo "a 更大"; fi
来源：http://tom.xylfe.cn

[R09] 字符串比较
来源：http://nwg.dianchejie.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gqo.jlsjyb.cn

[R10] 正则匹配
来源：http://obl.shanyushiyangtech.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gwy.xziqi.cn

[R11] case 多分支
来源：http://lth.jyoumei.cn

case "$1" in
来源：http://blp.aibaodan.cn

start) echo "启动" ;;
来源：http://bby.yanxiufei.cn

stop)  echo "停止" ;;
来源：http://jca.jinqigfzy.top

*)     echo "未知命令" ;;
来源：http://ksv.zdbjq.cn

esac
来源：http://epg.jqgufenzy.top

[R12] for 遍历文件
来源：http://iuq.hongshengwenyu.top

for f in *.txt; do echo "$f"; done
来源：http://zoz.hysaishi.cn

[R13] for 计数循环
来源：http://ubh.kuanghao11.cn

for i in {1..10}; do echo "$i"; done
来源：http://ieg.ctjpmb.com

[R14] C 风格 for
来源：http://auh.hesvh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rsz.hammf.cn

[R15] while 逐行读文件
来源：http://kft.hammf.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zuo.zdbjq.cn

[R16] until 等待条件
来源：http://xgl.yueranfly.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jgn.dianchejie.cn

[R17] 数组定义与取值
来源：http://ens.redwolf501.top

arr=(a b c); echo "${arr[0]}"
来源：http://qcf.ivvv.top

[R18] 遍历数组
来源：http://wsv.hcnkem.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qzl.yuanzhike.top

[R19] 数组长度
来源：http://cwu.cdnleiting.top

echo "${#arr[@]}"
来源：http://fnw.fehbvm.com

[R20] 关联数组（字典）
来源：http://jov.andypj.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://cuy.52xcode.cn

[R21] 字符串长度
来源：http://fyo.snrcjt.cn

echo "${#s}"
来源：http://biw.yfazqb.com

[R22] 截取子串
来源：http://vsn.jyoumei.cn

echo "${s:0:5}"
来源：http://zow.cheryme.top

[R23] 字符串替换
来源：http://mjj.sufxvd.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://zfz.zhoulong.xyz

[R24] 大小写转换
来源：http://nrk.uphjek.com

echo "${s^^}"; echo "${s,,}"
来源：http://jcd.hcnkem.com

[R25] 去后缀 / 去前缀
来源：http://lmi.zdqjudy.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wog.bbcook.cn

[R26] 命令替换
来源：http://uei.wangdashe.top

now=$(date +%F); echo "$now"
来源：http://dtp.cheryme.top

[R27] 算术展开
来源：http://zqf.shangyingyoupin.top

echo $((1 + 2 * 3))
来源：http://voo.jinqigufen.top

[R28] 浮点运算
来源：http://jic.wangshuangyany.cn

echo "scale=2; 10/3" | bc
来源：http://rtf.birdmap.top

[R29] 定义函数
来源：http://exs.tianlin.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wdw.tian-w.cn

[R30] 函数返回状态码
来源：http://ovd.haohaochexian.top

f() { return 0; }; f || echo "失败了"
来源：http://jsk.9152youxi.cn

[R31] 局部变量
来源：http://qci.redwolf501.top

f() { local x=1; echo "$x"; }
来源：http://lhf.yangfankeji.com

[R32] 参数个数校验
来源：http://bzy.cucudq.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oci.c1oappe.top

[R33] 捕获错误并提示行号
来源：http://yow.zycfv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ygy.shangyingyoupin.top

[R34] 退出时清理
来源：http://gvg.chenlongwang.top

trap 'rm -f "$tmp"' EXIT
来源：http://loh.yfazqb.com

[R35] 后台执行并等待
来源：http://lvk.gaohongyu789.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rgq.smart0.xyz

[R36] 并发执行多个任务
来源：http://lrn.sweek.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mqv.birdmap.top

[R37] 把输出赋给变量
来源：http://gru.zycfv.cn

files=$(ls -1)
来源：http://dzu.ivvv.top

[R38] 管道串联
来源：http://iig.nanxuanxn.top

cat a.txt | grep -i error | wc -l
来源：http://ivq.zdqjudy.top

[R39] 重定向标准输出与错误
来源：http://prz.aizwys.cn

cmd > out.log 2>&1
来源：http://zvw.guannengcc.top

[R40] 追加写日志
来源：http://drq.wangshuangyany.cn

echo "log" >> out.log
来源：http://ptj.fengsongda.top

[R41] 丢弃输出
来源：http://bgp.shzxlz.cn

cmd >/dev/null 2>&1
来源：http://nuh.yj20258888.top

[R42] 输入重定向
来源：http://qbe.zycfv.cn

wc -l < a.txt
来源：http://mjd.fanxiaobao.xyz

[R43] 按名字查找文件
来源：http://ayi.hongshengwenyu.top

find . -name "*.log" -type f
来源：http://hkf.jinqigufen.top

[R44] 按修改时间查找
来源：http://wup.quarkkingdee.top

find . -mtime -7 -type f
来源：http://iev.jinyuanbaomall.cn

[R45] 批量删除
来源：http://rac.pengpengdd.cyou

find . -name "*.tmp" -delete
来源：http://apv.jinqigfzy.top

[R46] 递归替换文件内容
来源：http://hnl.nanxinkj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fdt.tanke756.top

[R47] sed 单行替换
来源：http://yyh.epnwcf.com

sed -i 's/foo/bar/g' a.txt
来源：http://xra.shanyushiyangkeji.top

[R48] awk 取指定列
来源：http://kaj.guowangkeji.top

awk '{print $1, $3}' a.txt
来源：http://yfz.jqgufenzy.top

[R49] awk 带条件
来源：http://zsp.pengpengdd.cyou

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oks.ydzc1.top

[R50] awk 求和
来源：http://vvu.feifeiyinyue.top

awk '{s += $2} END {print s}' a.txt
来源：http://qls.yfazqb.com

[R51] 排序去重取前几
来源：http://tii.hongshengwenyu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cpa.yvedp.cn

[R52] 统计行数
来源：http://vbj.cucudq.cn

wc -l a.txt
来源：http://kfm.svipenyu.cn

[R53] 查看文件头与实时尾
来源：http://lhz.gogol.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uuj.dianchejie.cn

[R54] 比较两个文件
来源：http://mfi.zdbjq.cn

diff a.txt b.txt
来源：http://egi.xinyue.icu

[R55] 压缩与解压
来源：http://ryc.pengpengdd.cyou

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yfq.zdbjq.cn

[R56] 远程拷贝
来源：http://ggb.zhengqikj.top

scp file user@host:/path/
来源：http://als.yj20258.top

[R57] 远程执行命令
来源：http://rgd.ywan-chungtsiang.top

ssh user@host 'uptime'
来源：http://oli.jqgufenzy.top

[R58] 下载文件
来源：http://kfo.zhiwuduotai.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uqy.ctjpmb.com

[R59] 发 POST JSON
来源：http://ofr.xuanzx.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gje.svipenyu.cn

[R60] 只看 HTTP 状态码
来源：http://naz.uphjek.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dpr.yanxiufei.cn

[R61] 磁盘占用
来源：http://vna.yongpay.top

df -h;  du -sh *
来源：http://kci.xingfuxueyuan.xyz

[R62] 找最占空间的文件
来源：http://sos.shanyushiyangkeji.top

du -ah . | sort -rh | head -10
来源：http://dog.chenlongwang.top

[R63] 内存与进程
来源：http://bgp.jinqigfzy.top

free -h;  ps aux | grep nginx
来源：http://vzn.dianchejie.cn

[R64] 结束进程
来源：http://ksc.xinyue.icu

kill -9 $(pgrep -f app.py)
来源：http://koj.wangshuangyany.cn

[R65] 查看端口占用
来源：http://bag.tanke756.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cdj.jqgufenzy.top

[R66] 定时任务
来源：http://mzj.9152youxi.cn

crontab -e;  crontab -l
来源：http://mja.sufxvd.cn

[R67] 生成随机十六进制串
来源：http://gje.wangdashe.top

openssl rand -hex 16
来源：http://yqc.redwolf501.top

[R68] 计算文件校验值
来源：http://chm.xuetiantiany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gko.nanxuanxn.top

[R69] 生成随机密码
来源：http://txs.shangyingyoupin.top

head -c 16 /dev/urandom | base64
来源：http://ppw.jinqigufen.top

[R70] 时间戳与互转
来源：http://eln.hysaishi.cn

date +%s;  date -d @1700000000
来源：http://pbx.fehbvm.com

[R71] 日期格式化
来源：http://xkj.shanyushiyangkeji.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://apc.jianghu66.top

[R72] 等待端口就绪
来源：http://hpk.yongpay.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ggw.yuxming.cn

[R73] 分割大日志
来源：http://trt.52xcode.cn

split -l 1000 big.log part_
来源：http://ksy.ppjwa.cn

[R74] 批量重命名
来源：http://ioy.fengsongda.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ezm.nwbrower.top

[R75] 导出环境变量
来源：http://ptd.nanxinkj.top

export PATH="$HOME/bin:$PATH"
来源：http://hnt.pycfn.com

[R76] 使用临时文件
来源：http://kis.jinqigfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://str.zdqjudy.top

[R77] 读取用户输入
来源：http://hus.ivvv.top

read -rp "请输入: " ans
来源：http://xvq.hesvh.cn

[R78] 交互式菜单
来源：http://uzj.nanxuanxn.top

select opt in a b c; do echo "$opt"; break; done
来源：http://ymb.xziqi.cn

[R79] 解析命令行选项
来源：http://yql.fzhhl.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://otm.andypj.xyz

[R80] 查看脚本执行耗时
来源：http://ylc.xuetiantiany.cn

time ./run.sh
来源：http://hix.ydzc1.top

================================================================================
来源：http://sio.hnxiangtu.top

S. C / C++ 专题
来源：http://wpi.aibaodan.cn

================================================================================
来源：http://lso.ybcxt.top

[S01] C：Hello World
来源：http://ucu.zhaomingkeji.xyz

#include <stdio.h>
来源：http://uoy.cucudq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rsj.bjfxy.top

[S02] C：变量与格式化输出
来源：http://ikv.shzxlz.cn

int a = 10; printf("%d\n", a);
来源：http://mtj.shanyushiyangkeji.top

[S03] C：读入整数
来源：http://scx.cqqwz.cn

int x; scanf("%d", &x);
来源：http://fiw.zhongyouzk.top

[S04] C：字符串复制
来源：http://hls.shuidangran.top

char dst[32]; strcpy(dst, "hi");
来源：http://uix.yongpay.top

[S05] C：字符串长度
来源：http://stt.0kj1m.cn

strlen(s)
来源：http://ufb.vqdsnc.cn

[S06] C：字符串比较
来源：http://uew.yfazqb.com

strcmp(a, b) == 0
来源：http://txj.sjlbkw.cn

[S07] C：数组遍历求和
来源：http://xbn.fktsv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ino.aizwys.cn

[S08] C：动态内存分配与释放
来源：http://lle.9152youxi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dyp.yangfankeji.com

[S09] C：结构体定义与初始化
来源：http://zed.fktsv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://azp.chenjidiqi.icu

[S10] C：指针与解引用
来源：http://via.c1oappe.top

int *p = &a;  *p = 5;
来源：http://nwf.9152youxi.cn

[S11] C：逐行读文件
来源：http://btb.dianchejie.cn

FILE *f = fopen("a.txt", "r");
来源：http://iwz.jinghuilouyu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xby.yj20258888.top

fclose(f);
来源：http://bic.xylfe.cn

[S12] C：写文件
来源：http://idt.jinyuanbaomall.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ltm.ybcxt.top

[S13] C：宏定义
来源：http://xra.wangshuangyany.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yfr.316326.xyz

[S14] C：枚举
来源：http://cob.yuxming.cn

enum Color { RED, GREEN, BLUE };
来源：http://vqv.birdmap.top

[S15] C：类型转换
来源：http://hty.feifeiyinyue.top

(double) a / b
来源：http://hlp.uphjek.com

[S16] C：位操作置位
来源：http://hoe.wangdashe.top

x |= (1 << 3);
来源：http://djp.fzhhl.top

[S17] C：安全拼接字符串
来源：http://gal.fanxiaobao.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pgo.jianghu66.top

[S18] C：命令行参数
来源：http://jry.xinyue.icu

int main(int argc, char **argv)
来源：http://tha.jinghuilouyu.cn

[S19] C：快速排序
来源：http://zsz.cqqwz.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ahn.birdmap.top

[S20] C：二分查找
来源：http://wmb.52xcode.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gqp.cashguo.top

[S21] C：字符类别判断
来源：http://mfu.sufxvd.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bre.guowangkeji.top

[S22] C：字符串转数字
来源：http://mre.meibo888.top

atoi("42");  strtod("3.14", NULL);
来源：http://smz.chenlongwang.top

[S23] C：随机数
来源：http://zrt.sjlbkw.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://isa.cheryme.top

[S24] C：获取本地时间
来源：http://qbr.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mvd.hnqzz.top

[S25] C：内存拷贝
来源：http://htd.bjfxy.top

memcpy(dst, src, n);
来源：http://pqq.chenlongwang.top

[S26] C：内存清零
来源：http://abc.xylfe.cn

memset(a, 0, sizeof a);
来源：http://rms.tarul.cn

[S27] C：定义常量
来源：http://kkm.shzxlz.cn

const double PI = 3.14159;
来源：http://cza.ehwqpu.com

[S28] C：静态变量
来源：http://bum.yangfankeji.com

static int counter = 0;
来源：http://wzc.guannengcc.top

[S29] C：变参函数
来源：http://epc.hesvh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://obe.0kj1m.cn

[S30] C：头文件保护
来源：http://ery.yanxiufei.cn

#ifndef X_H
来源：http://mvw.gogol.net.cn

#define X_H
来源：http://byv.birdmap.top

#endif
来源：http://mjc.shuidangran.top

[S31] C++：Hello World
来源：http://glw.jianghu66.top

#include <iostream>
来源：http://cvz.zdqjudy.top

int main() { std::cout << "Hello\n"; }
来源：http://vqe.zhixingplan.top

[S32] C++：字符串
来源：http://tbx.xuetiantiany.cn

std::string s = "hi";  s += "!";
来源：http://jvx.birdmap.top

[S33] C++：vector 增删
来源：http://pfd.sxryk.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lxu.chenlongwang.top

[S34] C++：遍历 vector
来源：http://npn.wangshuangyany.cn

for (auto &x : v) { std::cout << x; }
来源：http://rii.bbcook.cn

[S35] C++：map
来源：http://hsf.cashguo.top

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tqz.yfazqb.com

[S36] C++：unordered_map
来源：http://ysw.ywan-chungtsiang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rnj.9152youxi.cn

[S37] C++：set
来源：http://jgw.shanyushiyangtech.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rxv.wangdashe.top

[S38] C++：排序
来源：http://sab.ywan-chungtsiang.top

std::sort(v.begin(), v.end());
来源：http://ete.dashuyun.cn

[S39] C++：自定义比较器排序
来源：http://qit.cqqwz.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hea.nanxuanxn.top

[S40] C++：查找元素
来源：http://vcv.fktsv.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://miy.epnwcf.com

[S41] C++：类与构造函数
来源：http://mii.jqgufenzy.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fbj.ppjwa.cn

[S42] C++：继承与虚函数
来源：http://niz.zhijiandao.cn

class B : public Base { public: void f() override {} };
来源：http://tyn.wangshuangyany.cn

[S43] C++：智能指针
来源：http://yti.yongpay.top

auto p = std::make_unique<int>(5);
来源：http://vsy.yfazqb.com

[S44] C++：引用传参
来源：http://qsv.wangshuangyany.cn

void inc(int &x) { ++x; }
来源：http://riz.jinqigufen.top

[S45] C++：lambda
来源：http://xjy.hesvh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zpz.cheryme.top

[S46] C++：函数模板
来源：http://zhk.shzxlz.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://nef.tianlin.xyz

[S47] C++：结构化绑定遍历
来源：http://aue.sweek.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nnk.jqgufenzy.top

[S48] C++：逐行读文件
来源：http://otp.mhx1999.top

std::ifstream in("a.txt");  std::string line;
来源：http://lve.vehdjk.com

while (std::getline(in, line)) { }
来源：http://nru.dashuyun.cn

[S49] C++：写文件
来源：http://wjs.zycfv.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cqj.c1oappe.top

[S50] C++：格式化数字
来源：http://vkw.jqgufenzy.top

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pfv.52xcode.cn

[S51] C++：显式类型转换
来源：http://lkk.jqgfzy.top

static_cast<double>(a) / b
来源：http://hpd.chenlongwang.top

[S52] C++：const 与 noexcept
来源：http://kyh.jinqigufen.top


<!-- 参考信息 -->