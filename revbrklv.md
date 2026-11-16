代发 wailian999

ROLLBACK TO sp1;
来源：http://ney.andypj.xyz

[Q69] 查看执行计划
来源：http://kvu.sysykeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ggt.xziqi.cn

[Q70] 更新统计信息
来源：http://fkj.guannengcc.top

ANALYZE TABLE users;
来源：http://erw.sjlbkw.cn

[Q71] 查看建表语句
来源：http://wth.hywenlv.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://sts.jianghu66.top

[Q72] 查看索引
来源：http://qxu.pycfn.com

SHOW INDEX FROM users;
来源：http://rvm.sjlbkw.cn

[Q73] 查看表状态
来源：http://tkp.yongpay.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mxb.daria6918.cn

[Q74] 强制使用索引
来源：http://yri.sjlbkw.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cwr.shuidangran.top

[Q75] 日期格式化
来源：http://wyf.316326.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mph.hesvh.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hmd.jinghuilouyu.cn

[Q76] 按天统计
来源：http://yex.yj202588.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zbj.sufxvd.cn

[Q77] 时间加减
来源：http://kgh.zhiwuduotai.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gxz.zhijiandao.cn

[Q78] 当前时间
来源：http://ujz.pengpengdd.cyou

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://uil.vqdsnc.cn

[Q79] 字符串拼接
来源：http://ioj.zhijiandao.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tmm.shanyushiyangtech.top

[Q80] 字符串截取
来源：http://qez.cheryme.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zpj.tianlin.xyz

[Q81] 字符串替换
来源：http://tnf.tian-w.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qta.guannengcc.top

[Q82] 字符长度与字节长度
来源：http://xum.jinqigufen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hou.gotoacloud.top

[Q83] 大小写转换
来源：http://yzc.gaohongyu789.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cpy.xylfe.cn

[Q84] 去除首尾空格
来源：http://gue.cdnleiting.top

SELECT TRIM(name) FROM users;
来源：http://nvp.yongpay.top

[Q85] 数值取整
来源：http://biv.cucudq.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yek.xziqi.cn

[Q86] 读取 JSON 字段
来源：http://vuh.kuanghao11.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://evo.hywenlv.cn

[Q87] JSON 字段做条件
来源：http://xtt.zhongyouzk.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zdl.quarkkingdee.top

[Q88] 行转列（条件聚合）
来源：http://ynf.xuanzx.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dso.hnxiangtu.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://shz.yonumen.top

[Q89] 判断表是否存在
来源：http://uvv.yuxming.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fqh.zdbjq.cn

[Q90] 生成序号列
来源：http://pfn.quarkkingdee.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://glq.shangyingyoupin.top

================================================================================
来源：http://evs.bjfxy.top

R. Bash 专题
来源：http://wrn.ydzc1.top

================================================================================
来源：http://vrh.zhijiandao.cn

[R01] shebang 与严格模式
来源：http://ypk.chenjidiqi.icu

#!/usr/bin/env bash
来源：http://ngy.guowangkeji.top

set -euo pipefail
来源：http://xix.redwolf501.top

[R02] 变量赋值与使用
来源：http://cfo.zycfv.cn

name="Tom"; echo "$name"
来源：http://rhl.andypj.xyz

[R03] 只读变量
来源：http://vvm.ppjwa.cn

readonly PI=3.14
来源：http://msq.gogol.net.cn

[R04] 位置参数
来源：http://tfy.jinqigufen.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://iky.andypj.xyz

[R05] 参数默认值
来源：http://cmh.xziqi.cn

name="${1:-default}"
来源：http://lwb.fanxiaobao.xyz

[R06] 判断命令是否存在
来源：http://qkf.yj20258.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://uoy.cashguo.top

[R07] if 判断文件
来源：http://nwv.zhiwuduotai.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jnl.ehwqpu.com

[R08] 数值比较
来源：http://wxw.ydzc1.top

if (( a > b )); then echo "a 更大"; fi
来源：http://rop.wangshuangyany.cn

[R09] 字符串比较
来源：http://itr.pengpengdd.cyou

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bgf.epnwcf.com

[R10] 正则匹配
来源：http://cls.meibo888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://tyg.hfpthk.cn

[R11] case 多分支
来源：http://vnk.sufxvd.cn

case "$1" in
来源：http://lbh.hammf.cn

start) echo "启动" ;;
来源：http://mqr.guowangkeji.top

stop)  echo "停止" ;;
来源：http://hfv.redwolf501.top

*)     echo "未知命令" ;;
来源：http://ovg.birdmap.top

esac
来源：http://htx.shuidangran.top

[R12] for 遍历文件
来源：http://phg.gogol.net.cn

for f in *.txt; do echo "$f"; done
来源：http://jtr.yj20258.top

[R13] for 计数循环
来源：http://wid.chenlongwang.top

for i in {1..10}; do echo "$i"; done
来源：http://pba.gzhubu.top

[R14] C 风格 for
来源：http://dsz.cdnleiting.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zbi.ydjk.org.cn

[R15] while 逐行读文件
来源：http://gon.jlsjyb.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fsp.sweek.top

[R16] until 等待条件
来源：http://llz.ybcxt.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kig.hammf.cn

[R17] 数组定义与取值
来源：http://ltx.ydjk.org.cn

arr=(a b c); echo "${arr[0]}"
来源：http://wkc.svipenyu.cn

[R18] 遍历数组
来源：http://tva.vqdsnc.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ito.daxiang520.top

[R19] 数组长度
来源：http://gyq.chenlongwang.top

echo "${#arr[@]}"
来源：http://mqv.dianchejie.cn

[R20] 关联数组（字典）
来源：http://cce.nanxinkj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://oth.bjfxy.top

[R21] 字符串长度
来源：http://rod.jqgufenzy.top

echo "${#s}"
来源：http://jml.yuanzhike.top

[R22] 截取子串
来源：http://syi.sysykeji.top

echo "${s:0:5}"
来源：http://qgb.fengsongda.top

[R23] 字符串替换
来源：http://sah.feifeiyinyue.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gft.gaohongyu789.top

[R24] 大小写转换
来源：http://kpw.havefunace.top

echo "${s^^}"; echo "${s,,}"
来源：http://xqm.sweek.top

[R25] 去后缀 / 去前缀
来源：http://eas.jinqigufen.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://skt.dashuyun.cn

[R26] 命令替换
来源：http://qfl.fzhhl.top

now=$(date +%F); echo "$now"
来源：http://xon.9152youxi.cn

[R27] 算术展开
来源：http://xth.xuanzx.com

echo $((1 + 2 * 3))
来源：http://hmz.shanyushiyangtech.top

[R28] 浮点运算
来源：http://bgd.gogol.net.cn

echo "scale=2; 10/3" | bc
来源：http://pnh.quarkkingdee.top

[R29] 定义函数
来源：http://rvb.daria6918.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://uzm.yonumen.top

[R30] 函数返回状态码
来源：http://kbe.nanxuanxn.top

f() { return 0; }; f || echo "失败了"
来源：http://bij.jqgfzy.top

[R31] 局部变量
来源：http://qbz.feifeiyinyue.top

f() { local x=1; echo "$x"; }
来源：http://nco.yuanzhike.top

[R32] 参数个数校验
来源：http://dzf.chenlongwang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://yxf.fzhhl.top

[R33] 捕获错误并提示行号
来源：http://zls.cashguo.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ohx.pengpengdd.cyou

[R34] 退出时清理
来源：http://ook.jqgufenzy.top

trap 'rm -f "$tmp"' EXIT
来源：http://uzt.shangyingyoupin.top

[R35] 后台执行并等待
来源：http://aqp.hongshengwenyu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://tir.jinqigufen.top

[R36] 并发执行多个任务
来源：http://mdv.vehdjk.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pme.fanxiaobao.xyz

[R37] 把输出赋给变量
来源：http://cfp.snrcjt.cn

files=$(ls -1)
来源：http://ocg.jinghuilouyu.cn

[R38] 管道串联
来源：http://rzr.pengpengdd.cyou

cat a.txt | grep -i error | wc -l
来源：http://pfg.xuetiantiany.cn

[R39] 重定向标准输出与错误
来源：http://lbm.wangdashe.top

cmd > out.log 2>&1
来源：http://bob.jqgfzy.top

[R40] 追加写日志
来源：http://svl.hammf.cn

echo "log" >> out.log
来源：http://eao.jiagoushi.top

[R41] 丢弃输出
来源：http://nji.zhoulong.xyz

cmd >/dev/null 2>&1
来源：http://rbj.hnqzz.top

[R42] 输入重定向
来源：http://qnj.cucudq.cn

wc -l < a.txt
来源：http://pwl.shangyingyoupin.top

[R43] 按名字查找文件
来源：http://jno.9152youxi.cn

find . -name "*.log" -type f
来源：http://zon.hammf.cn

[R44] 按修改时间查找
来源：http://sga.hfpthk.cn

find . -mtime -7 -type f
来源：http://gjs.shuidangran.top

[R45] 批量删除
来源：http://jfq.redwolf501.top

find . -name "*.tmp" -delete
来源：http://mrz.quarkkingdee.top

[R46] 递归替换文件内容
来源：http://uhq.xziqi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zgc.jqgufenzy.top

[R47] sed 单行替换
来源：http://ger.zhongyouzk.top

sed -i 's/foo/bar/g' a.txt
来源：http://ktn.dianchejie.cn

[R48] awk 取指定列
来源：http://omt.xziqi.cn

awk '{print $1, $3}' a.txt
来源：http://vpr.jqgufenzy.top

[R49] awk 带条件
来源：http://lte.zhijiandao.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jpp.c1oappe.top

[R50] awk 求和
来源：http://izm.vqdsnc.cn

awk '{s += $2} END {print s}' a.txt
来源：http://sim.shanyushiyangkeji.top

[R51] 排序去重取前几
来源：http://lnn.jinghuilouyu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://iua.xuetiantiany.cn

[R52] 统计行数
来源：http://tss.yueranfly.top

wc -l a.txt
来源：http://bes.xinyue.icu

[R53] 查看文件头与实时尾
来源：http://lys.gzhubu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hdp.nanxinkj.top

[R54] 比较两个文件
来源：http://brp.hammf.cn

diff a.txt b.txt
来源：http://ubw.nwbrower.top

[R55] 压缩与解压
来源：http://fyy.birdmap.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ozc.cucudq.cn

[R56] 远程拷贝
来源：http://tex.sxryk.cn

scp file user@host:/path/
来源：http://mhs.shuidangran.top

[R57] 远程执行命令
来源：http://oof.jiagoushi.top

ssh user@host 'uptime'
来源：http://bzv.xylfe.cn

[R58] 下载文件
来源：http://gpq.hcnkem.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uew.hongshengwenyu.top

[R59] 发 POST JSON
来源：http://rfj.fehbvm.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cwh.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://blv.hongshengwenyu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ggt.shuidangran.top

[R61] 磁盘占用
来源：http://vrj.gogol.net.cn

df -h;  du -sh *
来源：http://jby.redwolf501.top

[R62] 找最占空间的文件
来源：http://pjm.guannengcc.top

du -ah . | sort -rh | head -10
来源：http://hjw.bbcook.cn

[R63] 内存与进程
来源：http://eqt.kuanghao11.cn

free -h;  ps aux | grep nginx
来源：http://xbr.yuxming.cn

[R64] 结束进程
来源：http://fzf.jinqigufen.top

kill -9 $(pgrep -f app.py)
来源：http://pip.nanxuanxn.top

[R65] 查看端口占用
来源：http://qns.shangyingyoupin.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mlb.sxryk.cn

[R66] 定时任务
来源：http://nxg.ydjk.org.cn

crontab -e;  crontab -l
来源：http://ded.zhengqikj.top

[R67] 生成随机十六进制串
来源：http://ufw.jiagoushi.top

openssl rand -hex 16
来源：http://tmk.zhijiandao.cn

[R68] 计算文件校验值
来源：http://cpp.shzxlz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fku.zhaomingkeji.xyz

[R69] 生成随机密码
来源：http://tjv.sjlbkw.cn

head -c 16 /dev/urandom | base64
来源：http://ini.jyoumei.cn

[R70] 时间戳与互转
来源：http://vbg.ydjk.org.cn

date +%s;  date -d @1700000000
来源：http://fgu.sjlbkw.cn

[R71] 日期格式化
来源：http://dgb.gotoacloud.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://api.zhongyouzk.top

[R72] 等待端口就绪
来源：http://ynm.kuanghao11.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hxl.aizwys.cn

[R73] 分割大日志
来源：http://mfm.hcnkem.com

split -l 1000 big.log part_
来源：http://jla.zhaomingkeji.xyz

[R74] 批量重命名
来源：http://fki.pycfn.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cbd.vehdjk.com

[R75] 导出环境变量
来源：http://mae.guowangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://xxd.hesvh.cn

[R76] 使用临时文件
来源：http://kav.ehwqpu.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rty.hnqzz.top

[R77] 读取用户输入
来源：http://zhd.shuidangran.top

read -rp "请输入: " ans
来源：http://rwp.smart0.xyz

[R78] 交互式菜单
来源：http://dxn.gotoacloud.top

select opt in a b c; do echo "$opt"; break; done
来源：http://gug.xuanzx.com

[R79] 解析命令行选项
来源：http://sxu.daxiang520.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wrv.tianlin.xyz

[R80] 查看脚本执行耗时
来源：http://bcv.jqgfzy.top

time ./run.sh
来源：http://mnh.ehwqpu.com

================================================================================
来源：http://mtf.jinqigfzy.top

S. C / C++ 专题
来源：http://qoz.smart0.xyz

================================================================================
来源：http://jjg.yvedp.cn

[S01] C：Hello World
来源：http://zpa.xylfe.cn

#include <stdio.h>
来源：http://zrb.yueranfly.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fcr.xziqi.cn

[S02] C：变量与格式化输出
来源：http://xqi.gzhubu.top

int a = 10; printf("%d\n", a);
来源：http://tbk.guowangkeji.top

[S03] C：读入整数
来源：http://ner.andypj.xyz

int x; scanf("%d", &x);
来源：http://spq.ydjk.org.cn

[S04] C：字符串复制
来源：http://njo.zhoulong.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://pwi.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://zwt.andypj.xyz

strlen(s)
来源：http://zde.aibaodan.cn

[S06] C：字符串比较
来源：http://rix.chenlongwang.top

strcmp(a, b) == 0
来源：http://xdx.wangshuangyany.cn

[S07] C：数组遍历求和
来源：http://lwe.hnqzz.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vkc.52xcode.cn

[S08] C：动态内存分配与释放
来源：http://voq.sxryk.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gib.9152youxi.cn

[S09] C：结构体定义与初始化
来源：http://sxp.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zcr.nanxuanxn.top

[S10] C：指针与解引用
来源：http://yvc.ybcxt.top

int *p = &a;  *p = 5;
来源：http://joc.fanxiaobao.xyz

[S11] C：逐行读文件
来源：http://and.hcnkem.com

FILE *f = fopen("a.txt", "r");
来源：http://ysg.zhijiandao.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bkh.dianchejie.cn

fclose(f);
来源：http://lxp.hysaishi.cn

[S12] C：写文件
来源：http://bev.cdnleiting.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mas.xziqi.cn

[S13] C：宏定义
来源：http://goq.fzhhl.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wqs.jinghuilouyu.cn

[S14] C：枚举
来源：http://ybn.nanxuanxn.top

enum Color { RED, GREEN, BLUE };
来源：http://dtz.zhengqikj.top

[S15] C：类型转换
来源：http://vwj.redwolf501.top

(double) a / b
来源：http://ltg.jianghu66.top

[S16] C：位操作置位
来源：http://hgo.uphjek.com

x |= (1 << 3);
来源：http://bid.316326.xyz

[S17] C：安全拼接字符串
来源：http://uqf.guowangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kqq.fanxiaobao.xyz

[S18] C：命令行参数
来源：http://asd.aibaodan.cn

int main(int argc, char **argv)
来源：http://ath.redwolf501.top

[S19] C：快速排序
来源：http://zqw.sufxvd.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lcy.zhengqikj.top

[S20] C：二分查找
来源：http://eld.hammf.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ozl.hongshengwenyu.top

[S21] C：字符类别判断
来源：http://uwt.zdqjudy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jed.gogol.net.cn

[S22] C：字符串转数字
来源：http://nhd.jinqigufen.top

atoi("42");  strtod("3.14", NULL);
来源：http://ooh.wangshuangyany.cn

[S23] C：随机数
来源：http://irh.yj20258.top

srand(time(NULL));  int r = rand() % 100;
来源：http://yor.epnwcf.com

[S24] C：获取本地时间
来源：http://oei.tian-w.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bmd.ehwqpu.com

[S25] C：内存拷贝
来源：http://hak.jinqigfzy.top

memcpy(dst, src, n);
来源：http://tgb.fengsongda.top

[S26] C：内存清零
来源：http://amy.yuanzhike.top

memset(a, 0, sizeof a);
来源：http://dny.shanyushiyangtech.top

[S27] C：定义常量
来源：http://ghh.jinyuanbaomall.cn

const double PI = 3.14159;
来源：http://hcu.ctjpmb.com

[S28] C：静态变量
来源：http://gbi.yj202588.top

static int counter = 0;
来源：http://jsn.gaohongyu789.top

[S29] C：变参函数
来源：http://bza.wangdashe.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://evq.ehwqpu.com

[S30] C：头文件保护
来源：http://kfc.ydjk.org.cn

#ifndef X_H
来源：http://sjo.nanxinkj.top

#define X_H
来源：http://mom.nanxuanxn.top

#endif
来源：http://gwz.havefunace.top

[S31] C++：Hello World
来源：http://qtf.fktsv.cn

#include <iostream>
来源：http://sji.guowangkeji.top

int main() { std::cout << "Hello\n"; }
来源：http://fer.kuanghao11.cn

[S32] C++：字符串
来源：http://fcl.yfazqb.com

std::string s = "hi";  s += "!";
来源：http://rku.xylfe.cn

[S33] C++：vector 增删
来源：http://tfe.xingfuxueyuan.xyz

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ggy.yangfankeji.com

[S34] C++：遍历 vector
来源：http://cmb.hesvh.cn

for (auto &x : v) { std::cout << x; }
来源：http://bjv.jinghuilouyu.cn

[S35] C++：map
来源：http://rob.sufxvd.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aht.ywan-chungtsiang.top

[S36] C++：unordered_map
来源：http://bzd.uphjek.com

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nso.hfpthk.cn

[S37] C++：set
来源：http://nom.xingfuxueyuan.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lhc.mhx1999.top

[S38] C++：排序
来源：http://jdl.yueranfly.top

std::sort(v.begin(), v.end());
来源：http://vmt.yuanzhike.top


<!-- 参考信息 -->