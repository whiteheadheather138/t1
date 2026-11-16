代发 wailian999

[Q76] 按天统计
来源：http://bqj.yueranfly.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jkp.sjlbkw.cn

[Q77] 时间加减
来源：http://oie.pengpengdd.cyou

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://sam.fzhhl.top

[Q78] 当前时间
来源：http://cnj.yongpay.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://pof.svipenyu.cn

[Q79] 字符串拼接
来源：http://jzb.wangshuangyany.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://csx.uphjek.com

[Q80] 字符串截取
来源：http://ssj.zhoulong.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wua.yuanzhike.top

[Q81] 字符串替换
来源：http://eom.fehbvm.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://cft.hywenlv.cn

[Q82] 字符长度与字节长度
来源：http://ncw.sjlbkw.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://duj.shzxlz.cn

[Q83] 大小写转换
来源：http://mte.9152youxi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://jha.jinqigfzy.top

[Q84] 去除首尾空格
来源：http://ejb.sweek.top

SELECT TRIM(name) FROM users;
来源：http://mgz.cashguo.top

[Q85] 数值取整
来源：http://mnc.yvedp.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xny.aizwys.cn

[Q86] 读取 JSON 字段
来源：http://qqr.ybcxt.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://nso.pycfn.com

[Q87] JSON 字段做条件
来源：http://cij.haohaochexian.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rip.aizwys.cn

[Q88] 行转列（条件聚合）
来源：http://qzh.fehbvm.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://yex.shuidangran.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bvi.hcnkem.com

[Q89] 判断表是否存在
来源：http://vhj.haohaochexian.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mlp.bbcook.cn

[Q90] 生成序号列
来源：http://yuf.xinyue.icu

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hvj.sysykeji.top

================================================================================
来源：http://hiz.quarkkingdee.top

R. Bash 专题
来源：http://xfs.hnxiangtu.top

================================================================================
来源：http://sof.fehbvm.com

[R01] shebang 与严格模式
来源：http://bvq.nwbrower.top

#!/usr/bin/env bash
来源：http://mtc.dashuyun.cn

set -euo pipefail
来源：http://dsh.yuanzhike.top

[R02] 变量赋值与使用
来源：http://vak.hnxiangtu.top

name="Tom"; echo "$name"
来源：http://hxe.shanyushiyangkeji.top

[R03] 只读变量
来源：http://afk.fzhhl.top

readonly PI=3.14
来源：http://vxo.xylfe.cn

[R04] 位置参数
来源：http://omj.haohaochexian.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qso.sweek.top

[R05] 参数默认值
来源：http://fur.52xcode.cn

name="${1:-default}"
来源：http://wib.ydzc1.top

[R06] 判断命令是否存在
来源：http://hfr.jinqigufen.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ppz.nanxinkj.top

[R07] if 判断文件
来源：http://cqw.316326.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://brm.zhaomingkeji.xyz

[R08] 数值比较
来源：http://pwb.xingfuxueyuan.xyz

if (( a > b )); then echo "a 更大"; fi
来源：http://wsw.gogol.net.cn

[R09] 字符串比较
来源：http://fso.mhx1999.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://asx.chenzaomai.com

[R10] 正则匹配
来源：http://uvk.jinyuanbaomall.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jrz.yfazqb.com

[R11] case 多分支
来源：http://qgg.havefunace.top

case "$1" in
来源：http://gwy.316326.xyz

start) echo "启动" ;;
来源：http://hqg.vqdsnc.cn

stop)  echo "停止" ;;
来源：http://emu.cdnleiting.top

*)     echo "未知命令" ;;
来源：http://gib.wangdashe.top

esac
来源：http://tqg.c1oappe.top

[R12] for 遍历文件
来源：http://zll.yj20258888.top

for f in *.txt; do echo "$f"; done
来源：http://frq.tianlin.xyz

[R13] for 计数循环
来源：http://wry.iojbl.cn

for i in {1..10}; do echo "$i"; done
来源：http://xfm.tianlin.xyz

[R14] C 风格 for
来源：http://ret.cashguo.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bzd.shangyingyoupin.top

[R15] while 逐行读文件
来源：http://xhb.hammf.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://btu.shzxlz.cn

[R16] until 等待条件
来源：http://jfu.birdmap.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://dzd.ydzc1.top

[R17] 数组定义与取值
来源：http://ynn.cashguo.top

arr=(a b c); echo "${arr[0]}"
来源：http://vgd.snrcjt.cn

[R18] 遍历数组
来源：http://hvh.pycfn.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qry.dashuyun.cn

[R19] 数组长度
来源：http://sms.guowangkeji.top

echo "${#arr[@]}"
来源：http://xho.hfpthk.cn

[R20] 关联数组（字典）
来源：http://ybq.hywenlv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wcq.tanke756.top

[R21] 字符串长度
来源：http://sju.wangdashe.top

echo "${#s}"
来源：http://vxy.dashuyun.cn

[R22] 截取子串
来源：http://dsf.ydjk.org.cn

echo "${s:0:5}"
来源：http://pse.316326.xyz

[R23] 字符串替换
来源：http://yyn.jqgufenzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://guh.ydzc1.top

[R24] 大小写转换
来源：http://dfc.zdbjq.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lcs.aizwys.cn

[R25] 去后缀 / 去前缀
来源：http://upz.xinyue.icu

echo "${f%.txt}"; echo "${f#./}"
来源：http://wxv.sweek.top

[R26] 命令替换
来源：http://vyb.hammf.cn

now=$(date +%F); echo "$now"
来源：http://uoj.0kj1m.cn

[R27] 算术展开
来源：http://thw.wangshuangyany.cn

echo $((1 + 2 * 3))
来源：http://uyq.jinqigfzy.top

[R28] 浮点运算
来源：http://xky.vqdsnc.cn

echo "scale=2; 10/3" | bc
来源：http://cqg.hywenlv.cn

[R29] 定义函数
来源：http://ywl.hcnkem.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wva.chenlongwang.top

[R30] 函数返回状态码
来源：http://byk.havefunace.top

f() { return 0; }; f || echo "失败了"
来源：http://lnh.yuanzhike.top

[R31] 局部变量
来源：http://thc.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://dmp.cheryme.top

[R32] 参数个数校验
来源：http://dei.yangfankeji.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gos.sjlbkw.cn

[R33] 捕获错误并提示行号
来源：http://scv.xylfe.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rwa.tarul.cn

[R34] 退出时清理
来源：http://alx.shzxlz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mij.ehwqpu.com

[R35] 后台执行并等待
来源：http://bdm.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://mpf.jiagoushi.top

[R36] 并发执行多个任务
来源：http://oeq.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kjh.9152youxi.cn

[R37] 把输出赋给变量
来源：http://noj.daxiang520.top

files=$(ls -1)
来源：http://gym.ywan-chungtsiang.top

[R38] 管道串联
来源：http://row.hysaishi.cn

cat a.txt | grep -i error | wc -l
来源：http://uja.vehdjk.com

[R39] 重定向标准输出与错误
来源：http://nbn.yonumen.top

cmd > out.log 2>&1
来源：http://pol.gaohongyu789.top

[R40] 追加写日志
来源：http://fde.yueranfly.top

echo "log" >> out.log
来源：http://jab.tanke756.top

[R41] 丢弃输出
来源：http://tlm.bbcook.cn

cmd >/dev/null 2>&1
来源：http://lia.zhijiandao.cn

[R42] 输入重定向
来源：http://hal.hongshengwenyu.top

wc -l < a.txt
来源：http://zhe.shanyushiyangkeji.top

[R43] 按名字查找文件
来源：http://kku.cqqwz.cn

find . -name "*.log" -type f
来源：http://lle.sweek.top

[R44] 按修改时间查找
来源：http://siy.zhongyouzk.top

find . -mtime -7 -type f
来源：http://npq.birdmap.top

[R45] 批量删除
来源：http://vnn.ctjpmb.com

find . -name "*.tmp" -delete
来源：http://blh.zhoulong.xyz

[R46] 递归替换文件内容
来源：http://snd.dashuyun.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vlk.0kj1m.cn

[R47] sed 单行替换
来源：http://pyv.wangdashe.top

sed -i 's/foo/bar/g' a.txt
来源：http://ijs.andypj.xyz

[R48] awk 取指定列
来源：http://njy.zdqjudy.top

awk '{print $1, $3}' a.txt
来源：http://sur.xziqi.cn

[R49] awk 带条件
来源：http://alf.yj20258888.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yap.yuxming.cn

[R50] awk 求和
来源：http://hgh.jinghuilouyu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://iey.0kj1m.cn

[R51] 排序去重取前几
来源：http://fzd.yongpay.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cze.andypj.xyz

[R52] 统计行数
来源：http://pkc.ybcxt.top

wc -l a.txt
来源：http://oxi.jinqigfzy.top

[R53] 查看文件头与实时尾
来源：http://pce.smart0.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ybq.birdmap.top

[R54] 比较两个文件
来源：http://fsw.sjlbkw.cn

diff a.txt b.txt
来源：http://vro.hysaishi.cn

[R55] 压缩与解压
来源：http://syx.jinghuilouyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://isz.yonumen.top

[R56] 远程拷贝
来源：http://hel.xylfe.cn

scp file user@host:/path/
来源：http://xya.yj20258.top

[R57] 远程执行命令
来源：http://sok.snrcjt.cn

ssh user@host 'uptime'
来源：http://wtf.yfazqb.com

[R58] 下载文件
来源：http://ncj.svipenyu.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hyq.vehdjk.com

[R59] 发 POST JSON
来源：http://qol.kuanghao11.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wej.redwolf501.top

[R60] 只看 HTTP 状态码
来源：http://zkx.iojbl.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cmh.ctjpmb.com

[R61] 磁盘占用
来源：http://ivk.aizwys.cn

df -h;  du -sh *
来源：http://axw.yangfankeji.com

[R62] 找最占空间的文件
来源：http://ivg.jinqigfzy.top

du -ah . | sort -rh | head -10
来源：http://tts.cdnleiting.top

[R63] 内存与进程
来源：http://eii.xuanzx.com

free -h;  ps aux | grep nginx
来源：http://dgo.ydzc1.top

[R64] 结束进程
来源：http://mly.yj202588.top

kill -9 $(pgrep -f app.py)
来源：http://bop.fehbvm.com

[R65] 查看端口占用
来源：http://bkw.yuanzhike.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vvx.mhx1999.top

[R66] 定时任务
来源：http://sxf.zhiwuduotai.top

crontab -e;  crontab -l
来源：http://eho.hysaishi.cn

[R67] 生成随机十六进制串
来源：http://bjf.yangfankeji.com

openssl rand -hex 16
来源：http://qzp.tian-w.cn

[R68] 计算文件校验值
来源：http://tka.jqgfzy.top

sha256sum a.txt;  md5sum a.txt
来源：http://yrr.sxryk.cn

[R69] 生成随机密码
来源：http://bbn.jianghu66.top

head -c 16 /dev/urandom | base64
来源：http://krz.jlsjyb.cn

[R70] 时间戳与互转
来源：http://zwv.vqdsnc.cn

date +%s;  date -d @1700000000
来源：http://wdm.xinyue.icu

[R71] 日期格式化
来源：http://pgn.pycfn.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://lqn.fanxiaobao.xyz

[R72] 等待端口就绪
来源：http://eai.shzxlz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cir.hywenlv.cn

[R73] 分割大日志
来源：http://xtb.ybcxt.top

split -l 1000 big.log part_
来源：http://eyy.gzhubu.top

[R74] 批量重命名
来源：http://fxs.52xcode.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://acs.xziqi.cn

[R75] 导出环境变量
来源：http://hfn.andypj.xyz

export PATH="$HOME/bin:$PATH"
来源：http://rkv.zhaomingkeji.xyz

[R76] 使用临时文件
来源：http://ffj.hcnkem.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xbv.uphjek.com

[R77] 读取用户输入
来源：http://nsd.tarul.cn

read -rp "请输入: " ans
来源：http://tjp.chenzaomai.com

[R78] 交互式菜单
来源：http://clc.jqgfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://svx.smart0.xyz

[R79] 解析命令行选项
来源：http://tfv.aizwys.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://htp.hywenlv.cn

[R80] 查看脚本执行耗时
来源：http://dgm.zdbjq.cn

time ./run.sh
来源：http://jta.yueranfly.top

================================================================================
来源：http://jks.sxryk.cn

S. C / C++ 专题
来源：http://ere.wangshuangyany.cn

================================================================================
来源：http://cjk.nwbrower.top

[S01] C：Hello World
来源：http://blk.ydjk.org.cn

#include <stdio.h>
来源：http://kjn.ctjpmb.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://lvh.epnwcf.com

[S02] C：变量与格式化输出
来源：http://nfv.daxiang520.top

int a = 10; printf("%d\n", a);
来源：http://zej.daxiang520.top

[S03] C：读入整数
来源：http://zuc.meibo888.top

int x; scanf("%d", &x);
来源：http://qgb.wangdashe.top

[S04] C：字符串复制
来源：http://zdg.chenjidiqi.icu

char dst[32]; strcpy(dst, "hi");
来源：http://ikv.cucudq.cn

[S05] C：字符串长度
来源：http://hkw.xylfe.cn

strlen(s)
来源：http://rva.cucudq.cn

[S06] C：字符串比较
来源：http://uqn.andypj.xyz

strcmp(a, b) == 0
来源：http://dkn.fzhhl.top

[S07] C：数组遍历求和
来源：http://aes.jianghu66.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lwh.yuxming.cn

[S08] C：动态内存分配与释放
来源：http://umb.chenlongwang.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ixo.shanyushiyangtech.top

[S09] C：结构体定义与初始化
来源：http://gkg.xylfe.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qjy.hfpthk.cn

[S10] C：指针与解引用
来源：http://lbf.zdqjudy.top

int *p = &a;  *p = 5;
来源：http://cjm.zhijiandao.cn

[S11] C：逐行读文件
来源：http://bzp.haohaochexian.top

FILE *f = fopen("a.txt", "r");
来源：http://nub.shanyushiyangkeji.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://jbr.mhx1999.top

fclose(f);
来源：http://atz.xuanzx.com

[S12] C：写文件
来源：http://bak.gzhubu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://szm.gzhubu.top

[S13] C：宏定义
来源：http://xhe.yj20258.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pev.mhx1999.top

[S14] C：枚举
来源：http://hnd.yangfankeji.com

enum Color { RED, GREEN, BLUE };
来源：http://ywv.andypj.xyz

[S15] C：类型转换
来源：http://nhq.chenjidiqi.icu

(double) a / b
来源：http://xur.snrcjt.cn

[S16] C：位操作置位
来源：http://zpt.sxryk.cn

x |= (1 << 3);
来源：http://ixg.haohaochexian.top

[S17] C：安全拼接字符串
来源：http://ymy.yangfankeji.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jdr.gzhubu.top

[S18] C：命令行参数
来源：http://vxd.yueranfly.top

int main(int argc, char **argv)
来源：http://fmk.52xcode.cn

[S19] C：快速排序
来源：http://clv.meibo888.top

qsort(a, n, sizeof(int), cmp);
来源：http://lhd.ivvv.top

[S20] C：二分查找
来源：http://iyy.shangyingyoupin.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://bgc.shzxlz.cn

[S21] C：字符类别判断
来源：http://sor.hongshengwenyu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jyf.quarkkingdee.top

[S22] C：字符串转数字
来源：http://mjv.bjfxy.top

atoi("42");  strtod("3.14", NULL);
来源：http://roa.jlsjyb.cn

[S23] C：随机数
来源：http://vms.jqgfzy.top

srand(time(NULL));  int r = rand() % 100;
来源：http://apq.nanxuanxn.top

[S24] C：获取本地时间
来源：http://yvx.sysykeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ekf.dashuyun.cn

[S25] C：内存拷贝
来源：http://pyg.hnqzz.top

memcpy(dst, src, n);
来源：http://smm.316326.xyz

[S26] C：内存清零
来源：http://thc.tianlin.xyz

memset(a, 0, sizeof a);
来源：http://smx.iojbl.cn

[S27] C：定义常量
来源：http://ohw.nanxinkj.top

const double PI = 3.14159;
来源：http://jba.ivvv.top

[S28] C：静态变量
来源：http://fbi.zhaomingkeji.xyz

static int counter = 0;
来源：http://rze.bbcook.cn

[S29] C：变参函数
来源：http://gps.wangshuangyany.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://byj.sysykeji.top

[S30] C：头文件保护
来源：http://wfv.xuetiantiany.cn

#ifndef X_H
来源：http://ram.tanke756.top

#define X_H
来源：http://bvy.cheryme.top

#endif
来源：http://ytd.vqdsnc.cn

[S31] C++：Hello World
来源：http://izs.fengsongda.top

#include <iostream>
来源：http://uzx.hfpthk.cn

int main() { std::cout << "Hello\n"; }
来源：http://hem.sjlbkw.cn

[S32] C++：字符串
来源：http://xyo.wangdashe.top

std::string s = "hi";  s += "!";
来源：http://wqi.xuetiantiany.cn

[S33] C++：vector 增删
来源：http://lme.wangdashe.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lfm.kuanghao11.cn

[S34] C++：遍历 vector
来源：http://twi.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://wrz.xziqi.cn

[S35] C++：map
来源：http://emz.hcnkem.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://che.zhaomingkeji.xyz

[S36] C++：unordered_map
来源：http://its.c1oappe.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://llp.xingfuxueyuan.xyz

[S37] C++：set
来源：http://qzv.andypj.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jvp.c1oappe.top

[S38] C++：排序
来源：http://vfo.havefunace.top

std::sort(v.begin(), v.end());
来源：http://zxg.yonumen.top

[S39] C++：自定义比较器排序
来源：http://pqn.hfpthk.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lgk.daria6918.cn

[S40] C++：查找元素
来源：http://bua.iojbl.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gqn.yj202588.top

[S41] C++：类与构造函数
来源：http://css.xuanzx.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mtq.aibaodan.cn

[S42] C++：继承与虚函数
来源：http://aha.yongpay.top

class B : public Base { public: void f() override {} };
来源：http://wlw.wangdashe.top

[S43] C++：智能指针
来源：http://rpc.gzhubu.top

auto p = std::make_unique<int>(5);
来源：http://ufu.bjfxy.top

[S44] C++：引用传参
来源：http://aqp.hcnkem.com

void inc(int &x) { ++x; }
来源：http://krv.snrcjt.cn

[S45] C++：lambda
来源：http://mqm.tarul.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qxs.aizwys.cn

[S46] C++：函数模板
来源：http://pfl.316326.xyz

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cnj.jqgfzy.top


<!-- 参考信息 -->