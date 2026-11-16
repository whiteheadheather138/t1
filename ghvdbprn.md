代发 wailian999

[Q63] 开启事务
来源：http://agy.ehwqpu.com

START TRANSACTION;                -- 或 BEGIN
来源：http://kvc.wangshuangyany.cn

[Q64] 提交事务
来源：http://txx.52xcode.cn

COMMIT;
来源：http://opp.zhongyouzk.top

[Q65] 回滚事务
来源：http://eim.epnwcf.com

ROLLBACK;
来源：http://agt.52xcode.cn

[Q66] 行锁查询
来源：http://eyz.redwolf501.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xig.daxiang520.top

[Q67] 设置隔离级别
来源：http://kyg.cdnleiting.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bue.sufxvd.cn

[Q68] 保存点
来源：http://hsx.ppjwa.cn

SAVEPOINT sp1;
来源：http://ttp.shangyingyoupin.top

ROLLBACK TO sp1;
来源：http://xjx.hcnkem.com

[Q69] 查看执行计划
来源：http://xzr.jyoumei.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wol.yanxiufei.cn

[Q70] 更新统计信息
来源：http://gvl.c1oappe.top

ANALYZE TABLE users;
来源：http://rkp.shanyushiyangtech.top

[Q71] 查看建表语句
来源：http://ubf.hfpthk.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ttg.hongshengwenyu.top

[Q72] 查看索引
来源：http://lyc.bbcook.cn

SHOW INDEX FROM users;
来源：http://acp.cqqwz.cn

[Q73] 查看表状态
来源：http://edn.sufxvd.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gkg.yongpay.top

[Q74] 强制使用索引
来源：http://kwq.tianlin.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zci.epnwcf.com

[Q75] 日期格式化
来源：http://ofm.shuidangran.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ijw.haohaochexian.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hfz.zdqjudy.top

[Q76] 按天统计
来源：http://etf.tanke756.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fid.jinghuilouyu.cn

[Q77] 时间加减
来源：http://qam.ivvv.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ibi.jinyuanbaomall.cn

[Q78] 当前时间
来源：http://oma.snrcjt.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jqq.jianghu66.top

[Q79] 字符串拼接
来源：http://qho.sweek.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pki.yuanzhike.top

[Q80] 字符串截取
来源：http://rql.cdnleiting.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mql.guannengcc.top

[Q81] 字符串替换
来源：http://lbu.fanxiaobao.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hws.guannengcc.top

[Q82] 字符长度与字节长度
来源：http://bjc.xziqi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lhn.zhongyouzk.top

[Q83] 大小写转换
来源：http://smu.xuetiantiany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://stl.jiagoushi.top

[Q84] 去除首尾空格
来源：http://qpl.quarkkingdee.top

SELECT TRIM(name) FROM users;
来源：http://gtk.zhoulong.xyz

[Q85] 数值取整
来源：http://geu.nanxuanxn.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://asn.yonumen.top

[Q86] 读取 JSON 字段
来源：http://mem.sufxvd.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yyr.andypj.xyz

[Q87] JSON 字段做条件
来源：http://nsl.sysykeji.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mhu.yvedp.cn

[Q88] 行转列（条件聚合）
来源：http://ath.zhoulong.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://psz.shangyingyoupin.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://drz.zhixingplan.top

[Q89] 判断表是否存在
来源：http://eew.yj202588.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://trc.cucudq.cn

[Q90] 生成序号列
来源：http://foo.nwbrower.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nyq.fktsv.cn

================================================================================
来源：http://fja.shangyingyoupin.top

R. Bash 专题
来源：http://pnz.yj20258888.top

================================================================================
来源：http://atg.hfpthk.cn

[R01] shebang 与严格模式
来源：http://zmn.wangshuangyany.cn

#!/usr/bin/env bash
来源：http://lns.shzxlz.cn

set -euo pipefail
来源：http://fph.hnqzz.top

[R02] 变量赋值与使用
来源：http://nax.yanxiufei.cn

name="Tom"; echo "$name"
来源：http://kmb.316326.xyz

[R03] 只读变量
来源：http://qxg.nanxuanxn.top

readonly PI=3.14
来源：http://fgp.jqgufenzy.top

[R04] 位置参数
来源：http://pqi.zhengqikj.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fjf.sufxvd.cn

[R05] 参数默认值
来源：http://ugw.jinyuanbaomall.cn

name="${1:-default}"
来源：http://ydw.smart0.xyz

[R06] 判断命令是否存在
来源：http://pty.uphjek.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kyl.feifeiyinyue.top

[R07] if 判断文件
来源：http://zeb.xuetiantiany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dpb.dashuyun.cn

[R08] 数值比较
来源：http://erj.bbcook.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xrf.cdnleiting.top

[R09] 字符串比较
来源：http://uvk.guannengcc.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ggu.tian-w.cn

[R10] 正则匹配
来源：http://ygf.52xcode.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://urw.chenzaomai.com

[R11] case 多分支
来源：http://oau.fanxiaobao.xyz

case "$1" in
来源：http://mug.ybcxt.top

start) echo "启动" ;;
来源：http://nqo.pengpengdd.cyou

stop)  echo "停止" ;;
来源：http://ajr.pycfn.com

*)     echo "未知命令" ;;
来源：http://ohi.fzhhl.top

esac
来源：http://egn.jqgfzy.top

[R12] for 遍历文件
来源：http://ziy.yongpay.top

for f in *.txt; do echo "$f"; done
来源：http://oxa.sxryk.cn

[R13] for 计数循环
来源：http://emy.kuanghao11.cn

for i in {1..10}; do echo "$i"; done
来源：http://dce.cdnleiting.top

[R14] C 风格 for
来源：http://uwq.yuxming.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://lmq.ctjpmb.com

[R15] while 逐行读文件
来源：http://qfk.sufxvd.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sxn.jinghuilouyu.cn

[R16] until 等待条件
来源：http://pip.yj20258888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://acb.bbcook.cn

[R17] 数组定义与取值
来源：http://rtb.jiagoushi.top

arr=(a b c); echo "${arr[0]}"
来源：http://mbn.hnqzz.top

[R18] 遍历数组
来源：http://bsu.yvedp.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://khp.fehbvm.com

[R19] 数组长度
来源：http://qxo.bjfxy.top

echo "${#arr[@]}"
来源：http://zxb.shangyingyoupin.top

[R20] 关联数组（字典）
来源：http://bhs.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ejv.52xcode.cn

[R21] 字符串长度
来源：http://jgx.sufxvd.cn

echo "${#s}"
来源：http://kvf.andypj.xyz

[R22] 截取子串
来源：http://uuy.xinyue.icu

echo "${s:0:5}"
来源：http://eid.tanke756.top

[R23] 字符串替换
来源：http://bmm.ybcxt.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hpg.feifeiyinyue.top

[R24] 大小写转换
来源：http://scu.yuxming.cn

echo "${s^^}"; echo "${s,,}"
来源：http://adp.havefunace.top

[R25] 去后缀 / 去前缀
来源：http://ueg.fanxiaobao.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://qxi.yfazqb.com

[R26] 命令替换
来源：http://bav.tianlin.xyz

now=$(date +%F); echo "$now"
来源：http://oln.ppjwa.cn

[R27] 算术展开
来源：http://hqu.zhongyouzk.top

echo $((1 + 2 * 3))
来源：http://zwu.birdmap.top

[R28] 浮点运算
来源：http://yve.nanxuanxn.top

echo "scale=2; 10/3" | bc
来源：http://bkq.yj20258.top

[R29] 定义函数
来源：http://nsi.yuanzhike.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://smq.yj202588.top

[R30] 函数返回状态码
来源：http://vec.tian-w.cn

f() { return 0; }; f || echo "失败了"
来源：http://eie.birdmap.top

[R31] 局部变量
来源：http://kzj.yanxiufei.cn

f() { local x=1; echo "$x"; }
来源：http://duf.jqgfzy.top

[R32] 参数个数校验
来源：http://woc.chenjidiqi.icu

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wkl.hysaishi.cn

[R33] 捕获错误并提示行号
来源：http://isz.nanxuanxn.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ocu.vqdsnc.cn

[R34] 退出时清理
来源：http://qtm.fktsv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://adc.52xcode.cn

[R35] 后台执行并等待
来源：http://bud.fzhhl.top

sleep 5 & pid=$!; wait "$pid"
来源：http://uzm.zdqjudy.top

[R36] 并发执行多个任务
来源：http://bcp.zhiwuduotai.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ooi.cashguo.top

[R37] 把输出赋给变量
来源：http://hyb.fktsv.cn

files=$(ls -1)
来源：http://lkb.jinghuilouyu.cn

[R38] 管道串联
来源：http://ztm.bjfxy.top

cat a.txt | grep -i error | wc -l
来源：http://awy.hysaishi.cn

[R39] 重定向标准输出与错误
来源：http://ixx.hnqzz.top

cmd > out.log 2>&1
来源：http://smy.zhiwuduotai.top

[R40] 追加写日志
来源：http://wnd.hywenlv.cn

echo "log" >> out.log
来源：http://sbf.meibo888.top

[R41] 丢弃输出
来源：http://uxv.yuxming.cn

cmd >/dev/null 2>&1
来源：http://boc.shzxlz.cn

[R42] 输入重定向
来源：http://kxb.zhoulong.xyz

wc -l < a.txt
来源：http://zat.chenlongwang.top

[R43] 按名字查找文件
来源：http://rki.jinghuilouyu.cn

find . -name "*.log" -type f
来源：http://hac.sweek.top

[R44] 按修改时间查找
来源：http://sho.xuanzx.com

find . -mtime -7 -type f
来源：http://pth.jiagoushi.top

[R45] 批量删除
来源：http://omw.jinghuilouyu.cn

find . -name "*.tmp" -delete
来源：http://jfl.fehbvm.com

[R46] 递归替换文件内容
来源：http://jkm.svipenyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ivi.gzhubu.top

[R47] sed 单行替换
来源：http://aev.zhaomingkeji.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://mot.bjfxy.top

[R48] awk 取指定列
来源：http://zhk.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://okv.pycfn.com

[R49] awk 带条件
来源：http://fao.xingfuxueyuan.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cha.vqdsnc.cn

[R50] awk 求和
来源：http://hcc.aibaodan.cn

awk '{s += $2} END {print s}' a.txt
来源：http://dyh.ybcxt.top

[R51] 排序去重取前几
来源：http://wog.cashguo.top

sort a.txt | uniq -c | sort -rn | head
来源：http://wpa.ydzc1.top

[R52] 统计行数
来源：http://zla.zhijiandao.cn

wc -l a.txt
来源：http://pbv.xinyue.icu

[R53] 查看文件头与实时尾
来源：http://kfp.jyoumei.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mdt.yongpay.top

[R54] 比较两个文件
来源：http://erf.ppjwa.cn

diff a.txt b.txt
来源：http://ono.ybcxt.top

[R55] 压缩与解压
来源：http://gia.ehwqpu.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xtz.wangdashe.top

[R56] 远程拷贝
来源：http://pym.gogol.net.cn

scp file user@host:/path/
来源：http://tnk.hywenlv.cn

[R57] 远程执行命令
来源：http://qzz.nanxinkj.top

ssh user@host 'uptime'
来源：http://try.cdnleiting.top

[R58] 下载文件
来源：http://gno.nanxuanxn.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://uns.gaohongyu789.top

[R59] 发 POST JSON
来源：http://dbj.andypj.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cmw.vqdsnc.cn

[R60] 只看 HTTP 状态码
来源：http://loy.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lxo.gzhubu.top

[R61] 磁盘占用
来源：http://rhd.tanke756.top

df -h;  du -sh *
来源：http://rlc.cdnleiting.top

[R62] 找最占空间的文件
来源：http://juk.daxiang520.top

du -ah . | sort -rh | head -10
来源：http://koj.yanxiufei.cn

[R63] 内存与进程
来源：http://ysl.ydjk.org.cn

free -h;  ps aux | grep nginx
来源：http://ces.9152youxi.cn

[R64] 结束进程
来源：http://ghe.vehdjk.com

kill -9 $(pgrep -f app.py)
来源：http://evc.9152youxi.cn

[R65] 查看端口占用
来源：http://ooc.jqgfzy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uuw.quarkkingdee.top

[R66] 定时任务
来源：http://vsk.havefunace.top

crontab -e;  crontab -l
来源：http://txm.bbcook.cn

[R67] 生成随机十六进制串
来源：http://hwj.yuanzhike.top

openssl rand -hex 16
来源：http://fib.vqdsnc.cn

[R68] 计算文件校验值
来源：http://iit.guannengcc.top

sha256sum a.txt;  md5sum a.txt
来源：http://igg.yj20258.top

[R69] 生成随机密码
来源：http://pqs.jqgfzy.top

head -c 16 /dev/urandom | base64
来源：http://djd.feifeiyinyue.top

[R70] 时间戳与互转
来源：http://for.ydzc1.top

date +%s;  date -d @1700000000
来源：http://xeb.cqqwz.cn

[R71] 日期格式化
来源：http://xul.iojbl.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fev.hongshengwenyu.top

[R72] 等待端口就绪
来源：http://avw.sxryk.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tiv.tarul.cn

[R73] 分割大日志
来源：http://mbe.nanxinkj.top

split -l 1000 big.log part_
来源：http://zyr.yangfankeji.com

[R74] 批量重命名
来源：http://eni.pengpengdd.cyou

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hqz.zhiwuduotai.top

[R75] 导出环境变量
来源：http://equ.0kj1m.cn

export PATH="$HOME/bin:$PATH"
来源：http://vjz.smart0.xyz

[R76] 使用临时文件
来源：http://dxg.guannengcc.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://czu.chenlongwang.top

[R77] 读取用户输入
来源：http://owk.jianghu66.top

read -rp "请输入: " ans
来源：http://yan.snrcjt.cn

[R78] 交互式菜单
来源：http://kgg.tarul.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nhn.yuanzhike.top

[R79] 解析命令行选项
来源：http://imc.fanxiaobao.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qmx.jianghu66.top

[R80] 查看脚本执行耗时
来源：http://oqt.tanke756.top

time ./run.sh
来源：http://ypu.bbcook.cn

================================================================================
来源：http://ilm.yj20258.top

S. C / C++ 专题
来源：http://fom.hysaishi.cn

================================================================================
来源：http://qbc.jyoumei.cn

[S01] C：Hello World
来源：http://bil.yuxming.cn

#include <stdio.h>
来源：http://dtj.gotoacloud.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zlt.wangdashe.top

[S02] C：变量与格式化输出
来源：http://avk.cdnleiting.top

int a = 10; printf("%d\n", a);
来源：http://hio.52xcode.cn

[S03] C：读入整数
来源：http://zdw.kuanghao11.cn

int x; scanf("%d", &x);
来源：http://cjh.wangdashe.top

[S04] C：字符串复制
来源：http://ywm.jinqigfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://cpt.xingfuxueyuan.xyz

[S05] C：字符串长度
来源：http://bqn.zhaomingkeji.xyz

strlen(s)
来源：http://jve.bbcook.cn

[S06] C：字符串比较
来源：http://hwh.9152youxi.cn

strcmp(a, b) == 0
来源：http://wzr.aibaodan.cn

[S07] C：数组遍历求和
来源：http://phd.meibo888.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wng.zhijiandao.cn

[S08] C：动态内存分配与释放
来源：http://upd.hysaishi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://aym.meibo888.top

[S09] C：结构体定义与初始化
来源：http://lvd.ydzc1.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yjs.yanxiufei.cn

[S10] C：指针与解引用
来源：http://zpx.chenzaomai.com

int *p = &a;  *p = 5;
来源：http://bcz.jinghuilouyu.cn

[S11] C：逐行读文件
来源：http://ace.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://snq.xuetiantiany.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://pub.yj20258.top

fclose(f);
来源：http://oyd.xziqi.cn

[S12] C：写文件
来源：http://zts.ydzc1.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kws.jqgfzy.top

[S13] C：宏定义
来源：http://egq.pycfn.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xiq.yuxming.cn

[S14] C：枚举
来源：http://gzo.ehwqpu.com

enum Color { RED, GREEN, BLUE };
来源：http://sxf.fehbvm.com

[S15] C：类型转换
来源：http://bgr.shangyingyoupin.top

(double) a / b
来源：http://mie.daria6918.cn

[S16] C：位操作置位
来源：http://shh.sufxvd.cn

x |= (1 << 3);
来源：http://ofk.sysykeji.top

[S17] C：安全拼接字符串
来源：http://qdy.xziqi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bsc.wangshuangyany.cn

[S18] C：命令行参数
来源：http://kjf.sxryk.cn

int main(int argc, char **argv)
来源：http://jql.xuetiantiany.cn

[S19] C：快速排序
来源：http://uao.tianlin.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://pzl.ywan-chungtsiang.top

[S20] C：二分查找
来源：http://qub.fengsongda.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jwf.gzhubu.top

[S21] C：字符类别判断
来源：http://vhl.yueranfly.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://euh.jinqigufen.top

[S22] C：字符串转数字
来源：http://hzv.ywan-chungtsiang.top

atoi("42");  strtod("3.14", NULL);
来源：http://mwg.ywan-chungtsiang.top

[S23] C：随机数
来源：http://uns.hesvh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://rtr.tianlin.xyz

[S24] C：获取本地时间
来源：http://kxf.birdmap.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hnd.daxiang520.top

[S25] C：内存拷贝
来源：http://olr.jianghu66.top

memcpy(dst, src, n);
来源：http://taw.zhixingplan.top

[S26] C：内存清零
来源：http://nru.jinqigufen.top

memset(a, 0, sizeof a);
来源：http://eyv.fehbvm.com

[S27] C：定义常量
来源：http://rsp.yongpay.top

const double PI = 3.14159;
来源：http://xkk.shanyushiyangkeji.top

[S28] C：静态变量
来源：http://fsj.zdbjq.cn

static int counter = 0;
来源：http://pdj.redwolf501.top

[S29] C：变参函数
来源：http://gli.hywenlv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://emt.ywan-chungtsiang.top

[S30] C：头文件保护
来源：http://krb.yongpay.top

#ifndef X_H
来源：http://nnl.snrcjt.cn

#define X_H
来源：http://vwa.ydjk.org.cn

#endif
来源：http://pfm.xinyue.icu

[S31] C++：Hello World
来源：http://dqn.chenlongwang.top

#include <iostream>
来源：http://ztp.zhongyouzk.top

int main() { std::cout << "Hello\n"; }
来源：http://vvs.yonumen.top

[S32] C++：字符串
来源：http://dkg.zhengqikj.top

std::string s = "hi";  s += "!";
来源：http://rim.pycfn.com


<!-- 参考信息 -->