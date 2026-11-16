代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ehi.havefunace.top

[Q56] 密集排名（并列不占位）
来源：http://srw.fengsongda.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://izn.zycfv.cn

[Q57] 行号
来源：http://rhc.tianlin.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://avb.aibaodan.cn

[Q58] 累计求和
来源：http://wus.cucudq.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://fpg.jyoumei.cn

[Q59] 分组内累计
来源：http://nsc.smart0.xyz

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wga.guannengcc.top

[Q60] 取上一行 / 下一行
来源：http://vop.bjfxy.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://akh.cdnleiting.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mbf.cucudq.cn

[Q61] 移动平均
来源：http://crb.cashguo.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dik.yj20258888.top

[Q62] 分组占比
来源：http://vwm.cqqwz.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lkp.ehwqpu.com

[Q63] 开启事务
来源：http://iok.sjlbkw.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ntq.svipenyu.cn

[Q64] 提交事务
来源：http://mkw.hesvh.cn

COMMIT;
来源：http://vup.svipenyu.cn

[Q65] 回滚事务
来源：http://idp.ehwqpu.com

ROLLBACK;
来源：http://hev.aibaodan.cn

[Q66] 行锁查询
来源：http://hwb.cheryme.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://gvj.zhiwuduotai.top

[Q67] 设置隔离级别
来源：http://mre.xuetiantiany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://jgk.sufxvd.cn

[Q68] 保存点
来源：http://tuk.redwolf501.top

SAVEPOINT sp1;
来源：http://ghe.aibaodan.cn

ROLLBACK TO sp1;
来源：http://ptz.ydzc1.top

[Q69] 查看执行计划
来源：http://hyq.wangdashe.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://uob.zhijiandao.cn

[Q70] 更新统计信息
来源：http://xja.hesvh.cn

ANALYZE TABLE users;
来源：http://wxh.gzhubu.top

[Q71] 查看建表语句
来源：http://qfj.nanxuanxn.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nwu.jqgufenzy.top

[Q72] 查看索引
来源：http://gip.shanyushiyangtech.top

SHOW INDEX FROM users;
来源：http://bng.vqdsnc.cn

[Q73] 查看表状态
来源：http://ala.zhoulong.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://dys.jianghu66.top

[Q74] 强制使用索引
来源：http://fcv.hcnkem.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dcm.hnxiangtu.top

[Q75] 日期格式化
来源：http://mky.sxryk.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tkv.yueranfly.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ayl.ywan-chungtsiang.top

[Q76] 按天统计
来源：http://zil.pengpengdd.cyou

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://slk.kuanghao11.cn

[Q77] 时间加减
来源：http://noj.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ihn.ydjk.org.cn

[Q78] 当前时间
来源：http://hcm.c1oappe.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://muf.shangyingyoupin.top

[Q79] 字符串拼接
来源：http://kmh.hongshengwenyu.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://pht.tarul.cn

[Q80] 字符串截取
来源：http://zhj.ivvv.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dvo.xuanzx.com

[Q81] 字符串替换
来源：http://pfk.redwolf501.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://yyj.zhixingplan.top

[Q82] 字符长度与字节长度
来源：http://idm.aibaodan.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ndo.c1oappe.top

[Q83] 大小写转换
来源：http://rjq.jlsjyb.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qcl.ybcxt.top

[Q84] 去除首尾空格
来源：http://ylp.jinqigufen.top

SELECT TRIM(name) FROM users;
来源：http://ivm.jinghuilouyu.cn

[Q85] 数值取整
来源：http://gij.nwbrower.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cfy.pengpengdd.cyou

[Q86] 读取 JSON 字段
来源：http://dcd.yfazqb.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rsc.daxiang520.top

[Q87] JSON 字段做条件
来源：http://ioe.nanxinkj.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iou.zhijiandao.cn

[Q88] 行转列（条件聚合）
来源：http://ziv.redwolf501.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zpu.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xvm.xylfe.cn

[Q89] 判断表是否存在
来源：http://scg.fzhhl.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://byb.snrcjt.cn

[Q90] 生成序号列
来源：http://snh.hywenlv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kri.zdqjudy.top

================================================================================
来源：http://wff.kuanghao11.cn

R. Bash 专题
来源：http://xyl.nwbrower.top

================================================================================
来源：http://ufh.cucudq.cn

[R01] shebang 与严格模式
来源：http://bcu.guannengcc.top

#!/usr/bin/env bash
来源：http://dxk.chenlongwang.top

set -euo pipefail
来源：http://zjg.sysykeji.top

[R02] 变量赋值与使用
来源：http://ina.nwbrower.top

name="Tom"; echo "$name"
来源：http://iwp.ydjk.org.cn

[R03] 只读变量
来源：http://taj.ywan-chungtsiang.top

readonly PI=3.14
来源：http://twx.chenzaomai.com

[R04] 位置参数
来源：http://wbi.zycfv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cxp.sysykeji.top

[R05] 参数默认值
来源：http://wce.zycfv.cn

name="${1:-default}"
来源：http://big.nwbrower.top

[R06] 判断命令是否存在
来源：http://nfn.hnxiangtu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vwu.hysaishi.cn

[R07] if 判断文件
来源：http://gcs.aibaodan.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://oov.yanxiufei.cn

[R08] 数值比较
来源：http://far.c1oappe.top

if (( a > b )); then echo "a 更大"; fi
来源：http://eet.jqgfzy.top

[R09] 字符串比较
来源：http://qcx.uphjek.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://htm.jinqigufen.top

[R10] 正则匹配
来源：http://kky.dianchejie.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dnr.c1oappe.top

[R11] case 多分支
来源：http://eyv.guannengcc.top

case "$1" in
来源：http://bqu.yangfankeji.com

start) echo "启动" ;;
来源：http://eqg.52xcode.cn

stop)  echo "停止" ;;
来源：http://reo.316326.xyz

*)     echo "未知命令" ;;
来源：http://vgi.tarul.cn

esac
来源：http://skt.xziqi.cn

[R12] for 遍历文件
来源：http://fxg.hysaishi.cn

for f in *.txt; do echo "$f"; done
来源：http://fei.pengpengdd.cyou

[R13] for 计数循环
来源：http://lbh.kuanghao11.cn

for i in {1..10}; do echo "$i"; done
来源：http://uem.yonumen.top

[R14] C 风格 for
来源：http://tkb.xingfuxueyuan.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tvv.xziqi.cn

[R15] while 逐行读文件
来源：http://xme.zhixingplan.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lpo.jqgufenzy.top

[R16] until 等待条件
来源：http://scn.aibaodan.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://fxq.jqgfzy.top

[R17] 数组定义与取值
来源：http://rgb.ydzc1.top

arr=(a b c); echo "${arr[0]}"
来源：http://cex.ppjwa.cn

[R18] 遍历数组
来源：http://xaq.sweek.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rud.xylfe.cn

[R19] 数组长度
来源：http://wyd.birdmap.top

echo "${#arr[@]}"
来源：http://bwr.iojbl.cn

[R20] 关联数组（字典）
来源：http://hhi.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://dtp.yuanzhike.top

[R21] 字符串长度
来源：http://ohc.havefunace.top

echo "${#s}"
来源：http://epr.vehdjk.com

[R22] 截取子串
来源：http://juj.zycfv.cn

echo "${s:0:5}"
来源：http://wll.feifeiyinyue.top

[R23] 字符串替换
来源：http://lux.chenzaomai.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jeb.cdnleiting.top

[R24] 大小写转换
来源：http://vgs.wangdashe.top

echo "${s^^}"; echo "${s,,}"
来源：http://uvb.jyoumei.cn

[R25] 去后缀 / 去前缀
来源：http://amu.smart0.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://zxx.gzhubu.top

[R26] 命令替换
来源：http://roy.havefunace.top

now=$(date +%F); echo "$now"
来源：http://sxs.haohaochexian.top

[R27] 算术展开
来源：http://wuh.sjlbkw.cn

echo $((1 + 2 * 3))
来源：http://bbf.nanxuanxn.top

[R28] 浮点运算
来源：http://coi.bbcook.cn

echo "scale=2; 10/3" | bc
来源：http://kyh.9152youxi.cn

[R29] 定义函数
来源：http://aqm.jyoumei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qva.wangshuangyany.cn

[R30] 函数返回状态码
来源：http://ujf.guowangkeji.top

f() { return 0; }; f || echo "失败了"
来源：http://agw.zycfv.cn

[R31] 局部变量
来源：http://usn.chenjidiqi.icu

f() { local x=1; echo "$x"; }
来源：http://xgr.zycfv.cn

[R32] 参数个数校验
来源：http://nsv.xuetiantiany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://pti.sysykeji.top

[R33] 捕获错误并提示行号
来源：http://hrg.feifeiyinyue.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dml.jyoumei.cn

[R34] 退出时清理
来源：http://pet.havefunace.top

trap 'rm -f "$tmp"' EXIT
来源：http://kpx.andypj.xyz

[R35] 后台执行并等待
来源：http://igh.dashuyun.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fkt.yueranfly.top

[R36] 并发执行多个任务
来源：http://nem.snrcjt.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://orz.ybcxt.top

[R37] 把输出赋给变量
来源：http://bqg.jinyuanbaomall.cn

files=$(ls -1)
来源：http://nwd.yanxiufei.cn

[R38] 管道串联
来源：http://sea.shzxlz.cn

cat a.txt | grep -i error | wc -l
来源：http://ndt.c1oappe.top

[R39] 重定向标准输出与错误
来源：http://txs.zdbjq.cn

cmd > out.log 2>&1
来源：http://tvr.hywenlv.cn

[R40] 追加写日志
来源：http://quo.zhixingplan.top

echo "log" >> out.log
来源：http://xno.xuetiantiany.cn

[R41] 丢弃输出
来源：http://wpf.sysykeji.top

cmd >/dev/null 2>&1
来源：http://xhl.tanke756.top

[R42] 输入重定向
来源：http://tmg.fengsongda.top

wc -l < a.txt
来源：http://iyz.jqgufenzy.top

[R43] 按名字查找文件
来源：http://rqq.svipenyu.cn

find . -name "*.log" -type f
来源：http://xgi.ppjwa.cn

[R44] 按修改时间查找
来源：http://lup.ywan-chungtsiang.top

find . -mtime -7 -type f
来源：http://zog.xziqi.cn

[R45] 批量删除
来源：http://hnq.ehwqpu.com

find . -name "*.tmp" -delete
来源：http://zim.zhiwuduotai.top

[R46] 递归替换文件内容
来源：http://xgb.nanxinkj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://olh.kuanghao11.cn

[R47] sed 单行替换
来源：http://dto.ywan-chungtsiang.top

sed -i 's/foo/bar/g' a.txt
来源：http://uyd.fzhhl.top

[R48] awk 取指定列
来源：http://dxr.havefunace.top

awk '{print $1, $3}' a.txt
来源：http://xzw.yanxiufei.cn

[R49] awk 带条件
来源：http://pao.zhixingplan.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ubf.tian-w.cn

[R50] awk 求和
来源：http://xtv.yangfankeji.com

awk '{s += $2} END {print s}' a.txt
来源：http://ers.redwolf501.top

[R51] 排序去重取前几
来源：http://xvr.sxryk.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://spv.hysaishi.cn

[R52] 统计行数
来源：http://vip.shangyingyoupin.top

wc -l a.txt
来源：http://tnb.tanke756.top

[R53] 查看文件头与实时尾
来源：http://dnd.zhengqikj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fhq.tarul.cn

[R54] 比较两个文件
来源：http://bvt.wangdashe.top

diff a.txt b.txt
来源：http://chr.hnqzz.top

[R55] 压缩与解压
来源：http://csl.jinqigfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kgo.jqgfzy.top

[R56] 远程拷贝
来源：http://ujh.fanxiaobao.xyz

scp file user@host:/path/
来源：http://wgb.yj20258888.top

[R57] 远程执行命令
来源：http://esq.zhongyouzk.top

ssh user@host 'uptime'
来源：http://wbk.jianghu66.top

[R58] 下载文件
来源：http://cfq.xinyue.icu

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wgp.hammf.cn

[R59] 发 POST JSON
来源：http://byl.yonumen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://akb.hnxiangtu.top

[R60] 只看 HTTP 状态码
来源：http://syo.xingfuxueyuan.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fry.yanxiufei.cn

[R61] 磁盘占用
来源：http://muo.ybcxt.top

df -h;  du -sh *
来源：http://uws.uphjek.com

[R62] 找最占空间的文件
来源：http://txa.fzhhl.top

du -ah . | sort -rh | head -10
来源：http://mos.hywenlv.cn

[R63] 内存与进程
来源：http://mpo.jlsjyb.cn

free -h;  ps aux | grep nginx
来源：http://dpw.shanyushiyangtech.top

[R64] 结束进程
来源：http://dnu.xinyue.icu

kill -9 $(pgrep -f app.py)
来源：http://caq.ivvv.top

[R65] 查看端口占用
来源：http://bho.tian-w.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sgu.sweek.top

[R66] 定时任务
来源：http://khk.tianlin.xyz

crontab -e;  crontab -l
来源：http://uqb.gzhubu.top

[R67] 生成随机十六进制串
来源：http://ynl.tian-w.cn

openssl rand -hex 16
来源：http://csc.shanyushiyangkeji.top

[R68] 计算文件校验值
来源：http://cpv.havefunace.top

sha256sum a.txt;  md5sum a.txt
来源：http://avo.jqgufenzy.top

[R69] 生成随机密码
来源：http://wat.yvedp.cn

head -c 16 /dev/urandom | base64
来源：http://pyp.yangfankeji.com

[R70] 时间戳与互转
来源：http://iyk.redwolf501.top

date +%s;  date -d @1700000000
来源：http://vit.hongshengwenyu.top

[R71] 日期格式化
来源：http://waf.uphjek.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://kkt.jinyuanbaomall.cn

[R72] 等待端口就绪
来源：http://wrk.nanxuanxn.top

until nc -z localhost 3306; do sleep 1; done
来源：http://qed.ppjwa.cn

[R73] 分割大日志
来源：http://nnd.ybcxt.top

split -l 1000 big.log part_
来源：http://qtt.cqqwz.cn

[R74] 批量重命名
来源：http://uke.iojbl.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ljc.pengpengdd.cyou

[R75] 导出环境变量
来源：http://uox.gogol.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://ccf.jianghu66.top

[R76] 使用临时文件
来源：http://nxg.jinqigfzy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vck.jlsjyb.cn

[R77] 读取用户输入
来源：http://erj.zhiwuduotai.top

read -rp "请输入: " ans
来源：http://oce.cucudq.cn

[R78] 交互式菜单
来源：http://qlg.havefunace.top

select opt in a b c; do echo "$opt"; break; done
来源：http://vpi.shanyushiyangtech.top

[R79] 解析命令行选项
来源：http://bzl.tian-w.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xfi.sjlbkw.cn

[R80] 查看脚本执行耗时
来源：http://qsw.aizwys.cn

time ./run.sh
来源：http://plk.zhaomingkeji.xyz

================================================================================
来源：http://rie.chenjidiqi.icu

S. C / C++ 专题
来源：http://epz.shanyushiyangkeji.top

================================================================================
来源：http://lhw.zhiwuduotai.top

[S01] C：Hello World
来源：http://xnw.yj20258.top

#include <stdio.h>
来源：http://zcn.fzhhl.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zfc.daria6918.cn

[S02] C：变量与格式化输出
来源：http://pub.cashguo.top

int a = 10; printf("%d\n", a);
来源：http://cfv.meibo888.top

[S03] C：读入整数
来源：http://lzq.uphjek.com

int x; scanf("%d", &x);
来源：http://kvl.jinqigfzy.top

[S04] C：字符串复制
来源：http://xdb.ydjk.org.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uxv.xziqi.cn

[S05] C：字符串长度
来源：http://gio.feifeiyinyue.top

strlen(s)
来源：http://gdr.yangfankeji.com

[S06] C：字符串比较
来源：http://kgj.sxryk.cn

strcmp(a, b) == 0
来源：http://ngj.zhoulong.xyz

[S07] C：数组遍历求和
来源：http://gft.daxiang520.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wen.yj202588.top

[S08] C：动态内存分配与释放
来源：http://nta.redwolf501.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ate.0kj1m.cn

[S09] C：结构体定义与初始化
来源：http://oyp.yvedp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://enj.andypj.xyz

[S10] C：指针与解引用
来源：http://bnl.jlsjyb.cn

int *p = &a;  *p = 5;
来源：http://znp.yuxming.cn

[S11] C：逐行读文件
来源：http://vkx.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://dfp.jinyuanbaomall.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wth.fanxiaobao.xyz

fclose(f);
来源：http://kqc.shuidangran.top

[S12] C：写文件
来源：http://ynl.havefunace.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://btj.bjfxy.top

[S13] C：宏定义
来源：http://iik.shanyushiyangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hgs.yj20258888.top

[S14] C：枚举
来源：http://rzx.yuanzhike.top

enum Color { RED, GREEN, BLUE };
来源：http://kqp.ehwqpu.com

[S15] C：类型转换
来源：http://vqe.kuanghao11.cn

(double) a / b
来源：http://zqw.yfazqb.com

[S16] C：位操作置位
来源：http://sov.yj20258.top

x |= (1 << 3);
来源：http://tie.zhongyouzk.top

[S17] C：安全拼接字符串
来源：http://dic.bjfxy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://yoy.chenlongwang.top

[S18] C：命令行参数
来源：http://uzc.daxiang520.top

int main(int argc, char **argv)
来源：http://crd.jiagoushi.top

[S19] C：快速排序
来源：http://jli.mhx1999.top

qsort(a, n, sizeof(int), cmp);
来源：http://wgm.epnwcf.com

[S20] C：二分查找
来源：http://muu.chenzaomai.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oln.bbcook.cn

[S21] C：字符类别判断
来源：http://cel.ctjpmb.com

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nyl.zhengqikj.top

[S22] C：字符串转数字
来源：http://dyt.zhiwuduotai.top

atoi("42");  strtod("3.14", NULL);
来源：http://mhn.9152youxi.cn

[S23] C：随机数
来源：http://oox.xuetiantiany.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pan.pengpengdd.cyou

[S24] C：获取本地时间
来源：http://gol.bjfxy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://shb.yj20258.top

[S25] C：内存拷贝
来源：http://guv.yj20258888.top

memcpy(dst, src, n);
来源：http://zqj.316326.xyz

[S26] C：内存清零
来源：http://mgf.meibo888.top


<!-- 参考信息 -->