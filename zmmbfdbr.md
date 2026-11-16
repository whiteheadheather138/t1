代发 wailian999

[Q76] 按天统计
来源：http://gyl.jinghuilouyu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vyu.yj20258.top

[Q77] 时间加减
来源：http://muw.pycfn.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://efp.dashuyun.cn

[Q78] 当前时间
来源：http://gsk.xinyue.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ivs.ybcxt.top

[Q79] 字符串拼接
来源：http://qae.yj202588.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lyt.zhiwuduotai.top

[Q80] 字符串截取
来源：http://qxc.daria6918.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://quy.hesvh.cn

[Q81] 字符串替换
来源：http://por.yangfankeji.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://acz.zdbjq.cn

[Q82] 字符长度与字节长度
来源：http://zmw.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lrz.aibaodan.cn

[Q83] 大小写转换
来源：http://kjs.kuanghao11.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://lox.hysaishi.cn

[Q84] 去除首尾空格
来源：http://kwm.shzxlz.cn

SELECT TRIM(name) FROM users;
来源：http://rnm.c1oappe.top

[Q85] 数值取整
来源：http://zbf.vqdsnc.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jud.zhiwuduotai.top

[Q86] 读取 JSON 字段
来源：http://nhm.sufxvd.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ewd.shanyushiyangkeji.top

[Q87] JSON 字段做条件
来源：http://zhh.zhoulong.xyz

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rcx.jiagoushi.top

[Q88] 行转列（条件聚合）
来源：http://jcg.uphjek.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rnx.9152youxi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bbs.vqdsnc.cn

[Q89] 判断表是否存在
来源：http://yuy.yj20258.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fbn.chenjidiqi.icu

[Q90] 生成序号列
来源：http://cbr.jqgfzy.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://bnc.hywenlv.cn

================================================================================
来源：http://tld.feifeiyinyue.top

R. Bash 专题
来源：http://zwj.smart0.xyz

================================================================================
来源：http://nfn.fehbvm.com

[R01] shebang 与严格模式
来源：http://dfk.fengsongda.top

#!/usr/bin/env bash
来源：http://utw.yfazqb.com

set -euo pipefail
来源：http://yvu.xziqi.cn

[R02] 变量赋值与使用
来源：http://rri.wangdashe.top

name="Tom"; echo "$name"
来源：http://mav.shuidangran.top

[R03] 只读变量
来源：http://uij.tianlin.xyz

readonly PI=3.14
来源：http://bnj.guowangkeji.top

[R04] 位置参数
来源：http://vre.hnxiangtu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://zjf.dianchejie.cn

[R05] 参数默认值
来源：http://ywj.epnwcf.com

name="${1:-default}"
来源：http://xby.yuxming.cn

[R06] 判断命令是否存在
来源：http://icm.tanke756.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sqz.yongpay.top

[R07] if 判断文件
来源：http://lec.xingfuxueyuan.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://saw.bjfxy.top

[R08] 数值比较
来源：http://mcb.ydzc1.top

if (( a > b )); then echo "a 更大"; fi
来源：http://iey.cdnleiting.top

[R09] 字符串比较
来源：http://ddg.jianghu66.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://dis.shanyushiyangtech.top

[R10] 正则匹配
来源：http://cma.quarkkingdee.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xni.chenjidiqi.icu

[R11] case 多分支
来源：http://apd.hfpthk.cn

case "$1" in
来源：http://wdh.316326.xyz

start) echo "启动" ;;
来源：http://bdg.hammf.cn

stop)  echo "停止" ;;
来源：http://gsq.ydzc1.top

*)     echo "未知命令" ;;
来源：http://uqg.nwbrower.top

esac
来源：http://fvr.mhx1999.top

[R12] for 遍历文件
来源：http://dyk.gaohongyu789.top

for f in *.txt; do echo "$f"; done
来源：http://yuj.nanxinkj.top

[R13] for 计数循环
来源：http://toh.zhixingplan.top

for i in {1..10}; do echo "$i"; done
来源：http://ogq.shuidangran.top

[R14] C 风格 for
来源：http://pkv.zhijiandao.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ucx.hysaishi.cn

[R15] while 逐行读文件
来源：http://vyt.cashguo.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mfp.aizwys.cn

[R16] until 等待条件
来源：http://qsf.shzxlz.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://liw.aibaodan.cn

[R17] 数组定义与取值
来源：http://qln.snrcjt.cn

arr=(a b c); echo "${arr[0]}"
来源：http://auo.xinyue.icu

[R18] 遍历数组
来源：http://vlw.yvedp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wwp.cdnleiting.top

[R19] 数组长度
来源：http://zgo.iojbl.cn

echo "${#arr[@]}"
来源：http://pgp.ivvv.top

[R20] 关联数组（字典）
来源：http://zze.xuanzx.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oxj.yj202588.top

[R21] 字符串长度
来源：http://zbc.xuetiantiany.cn

echo "${#s}"
来源：http://bat.fktsv.cn

[R22] 截取子串
来源：http://ihm.jinghuilouyu.cn

echo "${s:0:5}"
来源：http://jcj.shuidangran.top

[R23] 字符串替换
来源：http://ngk.yfazqb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ydj.dianchejie.cn

[R24] 大小写转换
来源：http://cdz.hnqzz.top

echo "${s^^}"; echo "${s,,}"
来源：http://qxf.jiagoushi.top

[R25] 去后缀 / 去前缀
来源：http://iav.sjlbkw.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ruu.316326.xyz

[R26] 命令替换
来源：http://cwm.shanyushiyangkeji.top

now=$(date +%F); echo "$now"
来源：http://cyf.iojbl.cn

[R27] 算术展开
来源：http://llp.jiagoushi.top

echo $((1 + 2 * 3))
来源：http://fnk.shzxlz.cn

[R28] 浮点运算
来源：http://trk.jqgufenzy.top

echo "scale=2; 10/3" | bc
来源：http://zce.yangfankeji.com

[R29] 定义函数
来源：http://ojk.zhengqikj.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://lrs.hesvh.cn

[R30] 函数返回状态码
来源：http://kez.hnxiangtu.top

f() { return 0; }; f || echo "失败了"
来源：http://xpp.ctjpmb.com

[R31] 局部变量
来源：http://zrb.jinyuanbaomall.cn

f() { local x=1; echo "$x"; }
来源：http://yok.zhongyouzk.top

[R32] 参数个数校验
来源：http://oyc.jqgufenzy.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xkt.yvedp.cn

[R33] 捕获错误并提示行号
来源：http://tzz.52xcode.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://asw.hongshengwenyu.top

[R34] 退出时清理
来源：http://ijf.feifeiyinyue.top

trap 'rm -f "$tmp"' EXIT
来源：http://hjw.cucudq.cn

[R35] 后台执行并等待
来源：http://mlo.haohaochexian.top

sleep 5 & pid=$!; wait "$pid"
来源：http://gzt.redwolf501.top

[R36] 并发执行多个任务
来源：http://iky.dianchejie.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://jjd.c1oappe.top

[R37] 把输出赋给变量
来源：http://bhp.sjlbkw.cn

files=$(ls -1)
来源：http://nxp.yj202588.top

[R38] 管道串联
来源：http://srw.zhoulong.xyz

cat a.txt | grep -i error | wc -l
来源：http://njs.zhaomingkeji.xyz

[R39] 重定向标准输出与错误
来源：http://snz.pengpengdd.cyou

cmd > out.log 2>&1
来源：http://ihm.pengpengdd.cyou

[R40] 追加写日志
来源：http://coy.hammf.cn

echo "log" >> out.log
来源：http://pbv.shzxlz.cn

[R41] 丢弃输出
来源：http://msm.aizwys.cn

cmd >/dev/null 2>&1
来源：http://rpy.sysykeji.top

[R42] 输入重定向
来源：http://uex.yonumen.top

wc -l < a.txt
来源：http://avi.chenjidiqi.icu

[R43] 按名字查找文件
来源：http://tfo.sweek.top

find . -name "*.log" -type f
来源：http://joj.hammf.cn

[R44] 按修改时间查找
来源：http://dut.zhiwuduotai.top

find . -mtime -7 -type f
来源：http://dyr.dashuyun.cn

[R45] 批量删除
来源：http://wfk.cdnleiting.top

find . -name "*.tmp" -delete
来源：http://sqs.xinyue.icu

[R46] 递归替换文件内容
来源：http://ayy.hywenlv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ezk.hysaishi.cn

[R47] sed 单行替换
来源：http://gdw.ydzc1.top

sed -i 's/foo/bar/g' a.txt
来源：http://iie.fehbvm.com

[R48] awk 取指定列
来源：http://wps.shangyingyoupin.top

awk '{print $1, $3}' a.txt
来源：http://rjp.xziqi.cn

[R49] awk 带条件
来源：http://zoj.zhoulong.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yrd.fengsongda.top

[R50] awk 求和
来源：http://bft.hcnkem.com

awk '{s += $2} END {print s}' a.txt
来源：http://sma.ydjk.org.cn

[R51] 排序去重取前几
来源：http://xnx.jinyuanbaomall.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tgv.xziqi.cn

[R52] 统计行数
来源：http://bpp.cucudq.cn

wc -l a.txt
来源：http://opp.fehbvm.com

[R53] 查看文件头与实时尾
来源：http://twv.ybcxt.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rfq.ywan-chungtsiang.top

[R54] 比较两个文件
来源：http://kmx.xziqi.cn

diff a.txt b.txt
来源：http://xni.vqdsnc.cn

[R55] 压缩与解压
来源：http://zbp.pycfn.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qgl.birdmap.top

[R56] 远程拷贝
来源：http://vct.tarul.cn

scp file user@host:/path/
来源：http://hdl.epnwcf.com

[R57] 远程执行命令
来源：http://tns.316326.xyz

ssh user@host 'uptime'
来源：http://lhs.tanke756.top

[R58] 下载文件
来源：http://mdk.dianchejie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://tsa.hnqzz.top

[R59] 发 POST JSON
来源：http://gfu.cqqwz.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kyv.316326.xyz

[R60] 只看 HTTP 状态码
来源：http://tpc.yvedp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oux.zhiwuduotai.top

[R61] 磁盘占用
来源：http://yiu.pengpengdd.cyou

df -h;  du -sh *
来源：http://qyd.xinyue.icu

[R62] 找最占空间的文件
来源：http://xch.fzhhl.top

du -ah . | sort -rh | head -10
来源：http://hnd.ywan-chungtsiang.top

[R63] 内存与进程
来源：http://bto.shangyingyoupin.top

free -h;  ps aux | grep nginx
来源：http://pom.jiagoushi.top

[R64] 结束进程
来源：http://zug.snrcjt.cn

kill -9 $(pgrep -f app.py)
来源：http://aja.wangshuangyany.cn

[R65] 查看端口占用
来源：http://nkf.jyoumei.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qnh.xziqi.cn

[R66] 定时任务
来源：http://dlz.cashguo.top

crontab -e;  crontab -l
来源：http://foc.vqdsnc.cn

[R67] 生成随机十六进制串
来源：http://sgq.jinghuilouyu.cn

openssl rand -hex 16
来源：http://dmm.cashguo.top

[R68] 计算文件校验值
来源：http://dbo.yonumen.top

sha256sum a.txt;  md5sum a.txt
来源：http://mug.nwbrower.top

[R69] 生成随机密码
来源：http://xqo.chenjidiqi.icu

head -c 16 /dev/urandom | base64
来源：http://kwh.xylfe.cn

[R70] 时间戳与互转
来源：http://uvb.52xcode.cn

date +%s;  date -d @1700000000
来源：http://nhi.jyoumei.cn

[R71] 日期格式化
来源：http://ilr.zhijiandao.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://kuw.daria6918.cn

[R72] 等待端口就绪
来源：http://ppk.fanxiaobao.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://gdh.zhaomingkeji.xyz

[R73] 分割大日志
来源：http://soq.sweek.top

split -l 1000 big.log part_
来源：http://jjc.ppjwa.cn

[R74] 批量重命名
来源：http://ztf.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dux.316326.xyz

[R75] 导出环境变量
来源：http://kyr.havefunace.top

export PATH="$HOME/bin:$PATH"
来源：http://ghj.feifeiyinyue.top

[R76] 使用临时文件
来源：http://qcf.jinghuilouyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hho.shzxlz.cn

[R77] 读取用户输入
来源：http://zwb.zhixingplan.top

read -rp "请输入: " ans
来源：http://keu.guowangkeji.top

[R78] 交互式菜单
来源：http://fah.yj20258888.top

select opt in a b c; do echo "$opt"; break; done
来源：http://wfg.vehdjk.com

[R79] 解析命令行选项
来源：http://pcj.zhixingplan.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jbw.xuetiantiany.cn

[R80] 查看脚本执行耗时
来源：http://juy.zhaomingkeji.xyz

time ./run.sh
来源：http://bjt.shuidangran.top

================================================================================
来源：http://jjj.hnqzz.top

S. C / C++ 专题
来源：http://sco.zdbjq.cn

================================================================================
来源：http://ikp.redwolf501.top

[S01] C：Hello World
来源：http://vbw.fzhhl.top

#include <stdio.h>
来源：http://bsw.nanxuanxn.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://roq.jqgfzy.top

[S02] C：变量与格式化输出
来源：http://gho.vehdjk.com

int a = 10; printf("%d\n", a);
来源：http://uhi.tianlin.xyz

[S03] C：读入整数
来源：http://shs.sysykeji.top

int x; scanf("%d", &x);
来源：http://zsh.aibaodan.cn

[S04] C：字符串复制
来源：http://lxq.yanxiufei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lmi.sxryk.cn

[S05] C：字符串长度
来源：http://jue.zdbjq.cn

strlen(s)
来源：http://oaw.cashguo.top

[S06] C：字符串比较
来源：http://lmz.nanxuanxn.top

strcmp(a, b) == 0
来源：http://pdv.tanke756.top

[S07] C：数组遍历求和
来源：http://hpr.aizwys.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cff.tanke756.top

[S08] C：动态内存分配与释放
来源：http://uly.zhijiandao.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ypy.jinyuanbaomall.cn

[S09] C：结构体定义与初始化
来源：http://wik.zhaomingkeji.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uhw.iojbl.cn

[S10] C：指针与解引用
来源：http://zeb.vqdsnc.cn

int *p = &a;  *p = 5;
来源：http://bdq.nwbrower.top

[S11] C：逐行读文件
来源：http://jdi.xuanzx.com

FILE *f = fopen("a.txt", "r");
来源：http://vpw.chenjidiqi.icu

while (fgets(buf, sizeof buf, f)) { }
来源：http://rsg.zhongyouzk.top

fclose(f);
来源：http://qez.mhx1999.top

[S12] C：写文件
来源：http://jot.wangshuangyany.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iia.shuidangran.top

[S13] C：宏定义
来源：http://chw.shangyingyoupin.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jjl.yanxiufei.cn

[S14] C：枚举
来源：http://tau.iojbl.cn

enum Color { RED, GREEN, BLUE };
来源：http://rue.chenzaomai.com

[S15] C：类型转换
来源：http://ift.jqgufenzy.top

(double) a / b
来源：http://zqh.zdqjudy.top

[S16] C：位操作置位
来源：http://ixk.jlsjyb.cn

x |= (1 << 3);
来源：http://lrt.jlsjyb.cn

[S17] C：安全拼接字符串
来源：http://rwv.fzhhl.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xsc.sxryk.cn

[S18] C：命令行参数
来源：http://cie.yueranfly.top

int main(int argc, char **argv)
来源：http://jkw.hfpthk.cn

[S19] C：快速排序
来源：http://fyi.zycfv.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mka.sysykeji.top

[S20] C：二分查找
来源：http://xxo.shzxlz.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ovj.svipenyu.cn

[S21] C：字符类别判断
来源：http://inr.gotoacloud.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baz.zhaomingkeji.xyz

[S22] C：字符串转数字
来源：http://lyn.fengsongda.top

atoi("42");  strtod("3.14", NULL);
来源：http://huc.wangshuangyany.cn

[S23] C：随机数
来源：http://vxp.ivvv.top

srand(time(NULL));  int r = rand() % 100;
来源：http://iit.yj20258888.top

[S24] C：获取本地时间
来源：http://gny.shanyushiyangkeji.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fru.sufxvd.cn

[S25] C：内存拷贝
来源：http://eew.mhx1999.top

memcpy(dst, src, n);
来源：http://cal.tianlin.xyz

[S26] C：内存清零
来源：http://nbz.hesvh.cn

memset(a, 0, sizeof a);
来源：http://dxa.dashuyun.cn

[S27] C：定义常量
来源：http://dny.zhaomingkeji.xyz

const double PI = 3.14159;
来源：http://iqk.daria6918.cn

[S28] C：静态变量
来源：http://ivy.zdqjudy.top

static int counter = 0;
来源：http://hex.xziqi.cn

[S29] C：变参函数
来源：http://nfv.shangyingyoupin.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dkv.c1oappe.top

[S30] C：头文件保护
来源：http://uft.gogol.net.cn

#ifndef X_H
来源：http://wpj.ctjpmb.com

#define X_H
来源：http://tmw.feifeiyinyue.top

#endif
来源：http://xdd.iojbl.cn

[S31] C++：Hello World
来源：http://uyc.yongpay.top

#include <iostream>
来源：http://mbc.shangyingyoupin.top

int main() { std::cout << "Hello\n"; }
来源：http://med.guowangkeji.top

[S32] C++：字符串
来源：http://fmh.meibo888.top

std::string s = "hi";  s += "!";
来源：http://suu.ivvv.top

[S33] C++：vector 增删
来源：http://chb.fanxiaobao.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://krq.gzhubu.top

[S34] C++：遍历 vector
来源：http://lkq.sxryk.cn

for (auto &x : v) { std::cout << x; }
来源：http://ege.sweek.top

[S35] C++：map
来源：http://jkk.sxryk.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://cwv.vqdsnc.cn

[S36] C++：unordered_map
来源：http://fej.wangshuangyany.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xiz.jinghuilouyu.cn

[S37] C++：set
来源：http://dty.quarkkingdee.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tli.xinyue.icu

[S38] C++：排序
来源：http://kou.cheryme.top

std::sort(v.begin(), v.end());
来源：http://yqz.yonumen.top

[S39] C++：自定义比较器排序
来源：http://xgo.zdbjq.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bvc.jinqigufen.top

[S40] C++：查找元素
来源：http://qqh.cashguo.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mmj.jiagoushi.top

[S41] C++：类与构造函数
来源：http://fon.shanyushiyangtech.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wdp.gzhubu.top

[S42] C++：继承与虚函数
来源：http://sma.feifeiyinyue.top

class B : public Base { public: void f() override {} };
来源：http://cyn.yongpay.top

[S43] C++：智能指针
来源：http://ypt.jqgufenzy.top

auto p = std::make_unique<int>(5);
来源：http://tke.smart0.xyz

[S44] C++：引用传参
来源：http://cbc.sysykeji.top

void inc(int &x) { ++x; }
来源：http://ucc.yfazqb.com

[S45] C++：lambda
来源：http://ogj.hnxiangtu.top

auto add = [](int a, int b) { return a + b; };
来源：http://nol.vehdjk.com

[S46] C++：函数模板
来源：http://cfj.gogol.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ugp.yfazqb.com


<!-- 参考信息 -->