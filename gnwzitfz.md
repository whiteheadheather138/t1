代发 wailian999

[Q48] CTE 公用表表达式
来源：http://bnf.yueranfly.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://pee.hnqzz.top

SELECT * FROM t WHERE c > 5;
来源：http://ego.yangfankeji.com

[Q49] 更新单行
来源：http://yzp.havefunace.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://gvj.jyoumei.cn

[Q50] 批量更新
来源：http://qbn.sjlbkw.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://zol.uphjek.com

[Q51] 用子查询更新
来源：http://kxv.ivvv.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://jhm.andypj.xyz

[Q52] 删除指定行
来源：http://jvc.nanxinkj.top

DELETE FROM users WHERE id = 10;
来源：http://wqs.yvedp.cn

[Q53] 按条件删除
来源：http://yyl.hysaishi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://sum.sxryk.cn

[Q54] 清空表
来源：http://xlz.wangshuangyany.cn

TRUNCATE TABLE logs;
来源：http://cck.cheryme.top

[Q55] 排名（并列占位）
来源：http://qkx.fanxiaobao.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wix.sjlbkw.cn

[Q56] 密集排名（并列不占位）
来源：http://zgh.nanxuanxn.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://dhr.ywan-chungtsiang.top

[Q57] 行号
来源：http://vht.jyoumei.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uhb.shanyushiyangtech.top

[Q58] 累计求和
来源：http://xtf.shuidangran.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ium.yfazqb.com

[Q59] 分组内累计
来源：http://sjj.jinqigfzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dua.xziqi.cn

[Q60] 取上一行 / 下一行
来源：http://jtp.sufxvd.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://eyv.cheryme.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://jqk.shanyushiyangkeji.top

[Q61] 移动平均
来源：http://ees.yongpay.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tgd.guowangkeji.top

[Q62] 分组占比
来源：http://rva.bjfxy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://san.pycfn.com

[Q63] 开启事务
来源：http://tdy.sysykeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://uir.dashuyun.cn

[Q64] 提交事务
来源：http://jgh.tianlin.xyz

COMMIT;
来源：http://txl.pengpengdd.cyou

[Q65] 回滚事务
来源：http://egh.shuidangran.top

ROLLBACK;
来源：http://zkf.jiagoushi.top

[Q66] 行锁查询
来源：http://zqb.vehdjk.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://iiw.snrcjt.cn

[Q67] 设置隔离级别
来源：http://wrf.shanyushiyangtech.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vrr.hesvh.cn

[Q68] 保存点
来源：http://kkf.yangfankeji.com

SAVEPOINT sp1;
来源：http://zgj.tarul.cn

ROLLBACK TO sp1;
来源：http://ppp.chenjidiqi.icu

[Q69] 查看执行计划
来源：http://zjv.kuanghao11.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vrq.smart0.xyz

[Q70] 更新统计信息
来源：http://aae.ctjpmb.com

ANALYZE TABLE users;
来源：http://yqi.fzhhl.top

[Q71] 查看建表语句
来源：http://sce.ctjpmb.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cqx.wangshuangyany.cn

[Q72] 查看索引
来源：http://ftm.fengsongda.top

SHOW INDEX FROM users;
来源：http://gkg.ehwqpu.com

[Q73] 查看表状态
来源：http://tsc.316326.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://hik.yfazqb.com

[Q74] 强制使用索引
来源：http://ufq.jinyuanbaomall.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nyn.fengsongda.top

[Q75] 日期格式化
来源：http://bgz.yongpay.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cav.quarkkingdee.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://iyq.ctjpmb.com

[Q76] 按天统计
来源：http://jmx.ctjpmb.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://spy.xingfuxueyuan.xyz

[Q77] 时间加减
来源：http://lxh.tian-w.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ruw.jlsjyb.cn

[Q78] 当前时间
来源：http://ovt.cqqwz.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://llb.cqqwz.cn

[Q79] 字符串拼接
来源：http://ont.tianlin.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jfl.bbcook.cn

[Q80] 字符串截取
来源：http://bxf.yuanzhike.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uga.ydjk.org.cn

[Q81] 字符串替换
来源：http://upm.sysykeji.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://gew.sweek.top

[Q82] 字符长度与字节长度
来源：http://dyc.xingfuxueyuan.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://iqx.xinyue.icu

[Q83] 大小写转换
来源：http://dns.chenlongwang.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://anv.pycfn.com

[Q84] 去除首尾空格
来源：http://lhf.yj20258888.top

SELECT TRIM(name) FROM users;
来源：http://pyn.shuidangran.top

[Q85] 数值取整
来源：http://vxi.andypj.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bke.yangfankeji.com

[Q86] 读取 JSON 字段
来源：http://hog.zhoulong.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://twb.birdmap.top

[Q87] JSON 字段做条件
来源：http://gyj.dianchejie.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://woo.shanyushiyangkeji.top

[Q88] 行转列（条件聚合）
来源：http://lrk.vqdsnc.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://uhj.havefunace.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pft.zhijiandao.cn

[Q89] 判断表是否存在
来源：http://saj.kuanghao11.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qsj.gogol.net.cn

[Q90] 生成序号列
来源：http://pzl.feifeiyinyue.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uox.fktsv.cn

================================================================================
来源：http://knr.vehdjk.com

R. Bash 专题
来源：http://lsl.sweek.top

================================================================================
来源：http://yat.c1oappe.top

[R01] shebang 与严格模式
来源：http://rth.yongpay.top

#!/usr/bin/env bash
来源：http://ion.shangyingyoupin.top

set -euo pipefail
来源：http://emx.sysykeji.top

[R02] 变量赋值与使用
来源：http://plq.ppjwa.cn

name="Tom"; echo "$name"
来源：http://oya.ywan-chungtsiang.top

[R03] 只读变量
来源：http://zwi.yanxiufei.cn

readonly PI=3.14
来源：http://fks.0kj1m.cn

[R04] 位置参数
来源：http://iky.yonumen.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ytc.hnxiangtu.top

[R05] 参数默认值
来源：http://rud.zycfv.cn

name="${1:-default}"
来源：http://zzb.gaohongyu789.top

[R06] 判断命令是否存在
来源：http://oyc.uphjek.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ojw.ywan-chungtsiang.top

[R07] if 判断文件
来源：http://jis.iojbl.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nlm.epnwcf.com

[R08] 数值比较
来源：http://jcs.ydjk.org.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wql.dianchejie.cn

[R09] 字符串比较
来源：http://hjm.fehbvm.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://slf.xinyue.icu

[R10] 正则匹配
来源：http://xjq.jyoumei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rpk.jinghuilouyu.cn

[R11] case 多分支
来源：http://nht.yuanzhike.top

case "$1" in
来源：http://wwo.tianlin.xyz

start) echo "启动" ;;
来源：http://xno.jinghuilouyu.cn

stop)  echo "停止" ;;
来源：http://plg.yj202588.top

*)     echo "未知命令" ;;
来源：http://yqd.zdbjq.cn

esac
来源：http://eqh.snrcjt.cn

[R12] for 遍历文件
来源：http://btg.sysykeji.top

for f in *.txt; do echo "$f"; done
来源：http://unz.svipenyu.cn

[R13] for 计数循环
来源：http://ils.fzhhl.top

for i in {1..10}; do echo "$i"; done
来源：http://oqp.hysaishi.cn

[R14] C 风格 for
来源：http://iqe.meibo888.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://chm.zhoulong.xyz

[R15] while 逐行读文件
来源：http://dwm.tianlin.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://bdl.nanxinkj.top

[R16] until 等待条件
来源：http://ggr.tanke756.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://yhp.tanke756.top

[R17] 数组定义与取值
来源：http://hok.hesvh.cn

arr=(a b c); echo "${arr[0]}"
来源：http://gdr.cucudq.cn

[R18] 遍历数组
来源：http://ioz.mhx1999.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://twt.hywenlv.cn

[R19] 数组长度
来源：http://mko.yuanzhike.top

echo "${#arr[@]}"
来源：http://adh.ehwqpu.com

[R20] 关联数组（字典）
来源：http://xpi.nanxinkj.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gsy.quarkkingdee.top

[R21] 字符串长度
来源：http://deh.vqdsnc.cn

echo "${#s}"
来源：http://kmk.ivvv.top

[R22] 截取子串
来源：http://zem.mhx1999.top

echo "${s:0:5}"
来源：http://oqc.vqdsnc.cn

[R23] 字符串替换
来源：http://mpz.aibaodan.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vuu.chenzaomai.com

[R24] 大小写转换
来源：http://zth.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://vrt.yongpay.top

[R25] 去后缀 / 去前缀
来源：http://ioh.jlsjyb.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gvr.aizwys.cn

[R26] 命令替换
来源：http://bwx.andypj.xyz

now=$(date +%F); echo "$now"
来源：http://igv.ehwqpu.com

[R27] 算术展开
来源：http://tvu.guowangkeji.top

echo $((1 + 2 * 3))
来源：http://usa.kuanghao11.cn

[R28] 浮点运算
来源：http://mnb.tianlin.xyz

echo "scale=2; 10/3" | bc
来源：http://gpz.yanxiufei.cn

[R29] 定义函数
来源：http://nkg.yanxiufei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://tqc.tian-w.cn

[R30] 函数返回状态码
来源：http://dwl.yfazqb.com

f() { return 0; }; f || echo "失败了"
来源：http://txn.ivvv.top

[R31] 局部变量
来源：http://aof.daxiang520.top

f() { local x=1; echo "$x"; }
来源：http://bnq.xuanzx.com

[R32] 参数个数校验
来源：http://wdf.yueranfly.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://lot.nanxuanxn.top

[R33] 捕获错误并提示行号
来源：http://msc.cheryme.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rod.wangshuangyany.cn

[R34] 退出时清理
来源：http://wxx.gaohongyu789.top

trap 'rm -f "$tmp"' EXIT
来源：http://mlr.ppjwa.cn

[R35] 后台执行并等待
来源：http://tgp.yfazqb.com

sleep 5 & pid=$!; wait "$pid"
来源：http://bfi.svipenyu.cn

[R36] 并发执行多个任务
来源：http://wpq.sysykeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zmb.aibaodan.cn

[R37] 把输出赋给变量
来源：http://blx.xziqi.cn

files=$(ls -1)
来源：http://xir.yueranfly.top

[R38] 管道串联
来源：http://rre.316326.xyz

cat a.txt | grep -i error | wc -l
来源：http://tkz.yangfankeji.com

[R39] 重定向标准输出与错误
来源：http://qaq.nwbrower.top

cmd > out.log 2>&1
来源：http://eqi.gogol.net.cn

[R40] 追加写日志
来源：http://nhv.zhoulong.xyz

echo "log" >> out.log
来源：http://uci.vehdjk.com

[R41] 丢弃输出
来源：http://ige.vehdjk.com

cmd >/dev/null 2>&1
来源：http://pmk.ydjk.org.cn

[R42] 输入重定向
来源：http://fsu.nanxinkj.top

wc -l < a.txt
来源：http://adj.yj20258888.top

[R43] 按名字查找文件
来源：http://zhe.smart0.xyz

find . -name "*.log" -type f
来源：http://xex.mhx1999.top

[R44] 按修改时间查找
来源：http://sea.hammf.cn

find . -mtime -7 -type f
来源：http://oec.sweek.top

[R45] 批量删除
来源：http://hwb.hammf.cn

find . -name "*.tmp" -delete
来源：http://ymt.sxryk.cn

[R46] 递归替换文件内容
来源：http://wkj.hysaishi.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pfq.andypj.xyz

[R47] sed 单行替换
来源：http://bvl.ppjwa.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lnv.guannengcc.top

[R48] awk 取指定列
来源：http://qky.fengsongda.top

awk '{print $1, $3}' a.txt
来源：http://hgb.cqqwz.cn

[R49] awk 带条件
来源：http://gpx.316326.xyz

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gob.jqgfzy.top

[R50] awk 求和
来源：http://nkt.aibaodan.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bib.sweek.top

[R51] 排序去重取前几
来源：http://iiq.guowangkeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://pwg.yuxming.cn

[R52] 统计行数
来源：http://yob.chenjidiqi.icu

wc -l a.txt
来源：http://yyq.pengpengdd.cyou

[R53] 查看文件头与实时尾
来源：http://xxr.yj20258.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wrm.cqqwz.cn

[R54] 比较两个文件
来源：http://vdi.52xcode.cn

diff a.txt b.txt
来源：http://mwp.ctjpmb.com

[R55] 压缩与解压
来源：http://aqw.vehdjk.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mdd.pengpengdd.cyou

[R56] 远程拷贝
来源：http://zlj.havefunace.top

scp file user@host:/path/
来源：http://xgj.jinyuanbaomall.cn

[R57] 远程执行命令
来源：http://mqi.ivvv.top

ssh user@host 'uptime'
来源：http://dzv.52xcode.cn

[R58] 下载文件
来源：http://mlm.iojbl.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dum.yuanzhike.top

[R59] 发 POST JSON
来源：http://bzm.uphjek.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://afq.gzhubu.top

[R60] 只看 HTTP 状态码
来源：http://wdt.shuidangran.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cwn.mhx1999.top

[R61] 磁盘占用
来源：http://xzm.zhengqikj.top

df -h;  du -sh *
来源：http://jwq.iojbl.cn

[R62] 找最占空间的文件
来源：http://lxn.cheryme.top

du -ah . | sort -rh | head -10
来源：http://krf.fanxiaobao.xyz

[R63] 内存与进程
来源：http://gii.aibaodan.cn

free -h;  ps aux | grep nginx
来源：http://kjp.sufxvd.cn

[R64] 结束进程
来源：http://dih.guowangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://bga.zycfv.cn

[R65] 查看端口占用
来源：http://iqg.cashguo.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hri.hnqzz.top

[R66] 定时任务
来源：http://wiz.cucudq.cn

crontab -e;  crontab -l
来源：http://ruq.zhijiandao.cn

[R67] 生成随机十六进制串
来源：http://qno.jinqigfzy.top

openssl rand -hex 16
来源：http://lgx.sjlbkw.cn

[R68] 计算文件校验值
来源：http://dtw.zycfv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://kke.hammf.cn

[R69] 生成随机密码
来源：http://wbx.jinghuilouyu.cn

head -c 16 /dev/urandom | base64
来源：http://dhf.dashuyun.cn

[R70] 时间戳与互转
来源：http://ufb.fanxiaobao.xyz

date +%s;  date -d @1700000000
来源：http://mzg.yonumen.top

[R71] 日期格式化
来源：http://osc.yuxming.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hta.chenjidiqi.icu

[R72] 等待端口就绪
来源：http://bdy.fktsv.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vwx.epnwcf.com

[R73] 分割大日志
来源：http://gku.ywan-chungtsiang.top

split -l 1000 big.log part_
来源：http://piv.snrcjt.cn

[R74] 批量重命名
来源：http://pxq.zhixingplan.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fqv.yongpay.top

[R75] 导出环境变量
来源：http://avi.zhongyouzk.top

export PATH="$HOME/bin:$PATH"
来源：http://nte.yueranfly.top

[R76] 使用临时文件
来源：http://hxt.shzxlz.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rfg.gzhubu.top

[R77] 读取用户输入
来源：http://wjy.ctjpmb.com

read -rp "请输入: " ans
来源：http://asu.9152youxi.cn

[R78] 交互式菜单
来源：http://moh.chenlongwang.top

select opt in a b c; do echo "$opt"; break; done
来源：http://crv.ehwqpu.com

[R79] 解析命令行选项
来源：http://bxs.zhoulong.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ojy.tianlin.xyz

[R80] 查看脚本执行耗时
来源：http://pkj.xuetiantiany.cn

time ./run.sh
来源：http://kyx.havefunace.top

================================================================================
来源：http://hvy.tianlin.xyz

S. C / C++ 专题
来源：http://rvo.cucudq.cn

================================================================================
来源：http://jyc.xuetiantiany.cn

[S01] C：Hello World
来源：http://xnb.jiagoushi.top

#include <stdio.h>
来源：http://fhh.haohaochexian.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ovk.ppjwa.cn

[S02] C：变量与格式化输出
来源：http://vqw.meibo888.top

int a = 10; printf("%d\n", a);
来源：http://mof.dianchejie.cn

[S03] C：读入整数
来源：http://lww.chenlongwang.top

int x; scanf("%d", &x);
来源：http://pre.zhengqikj.top

[S04] C：字符串复制
来源：http://fwo.nanxuanxn.top

char dst[32]; strcpy(dst, "hi");
来源：http://pzc.ydjk.org.cn

[S05] C：字符串长度
来源：http://rbl.aibaodan.cn

strlen(s)
来源：http://kgi.ehwqpu.com

[S06] C：字符串比较
来源：http://dps.sweek.top

strcmp(a, b) == 0
来源：http://dek.jinghuilouyu.cn

[S07] C：数组遍历求和
来源：http://wbj.hongshengwenyu.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://swq.ctjpmb.com

[S08] C：动态内存分配与释放
来源：http://mxx.bjfxy.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cfc.jqgfzy.top

[S09] C：结构体定义与初始化
来源：http://rpr.hywenlv.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mxt.guowangkeji.top

[S10] C：指针与解引用
来源：http://uzf.snrcjt.cn

int *p = &a;  *p = 5;
来源：http://ier.birdmap.top

[S11] C：逐行读文件
来源：http://hyj.fktsv.cn

FILE *f = fopen("a.txt", "r");
来源：http://ysw.daria6918.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vnx.ivvv.top

fclose(f);
来源：http://pkr.xuanzx.com

[S12] C：写文件
来源：http://pkj.tanke756.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rsx.birdmap.top

[S13] C：宏定义
来源：http://hjx.daria6918.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vfa.c1oappe.top

[S14] C：枚举
来源：http://kxm.9152youxi.cn

enum Color { RED, GREEN, BLUE };
来源：http://xub.9152youxi.cn

[S15] C：类型转换
来源：http://wzq.quarkkingdee.top

(double) a / b
来源：http://mra.bjfxy.top

[S16] C：位操作置位
来源：http://lsi.fehbvm.com

x |= (1 << 3);
来源：http://lxc.tianlin.xyz

[S17] C：安全拼接字符串
来源：http://vgj.wangdashe.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gmf.ywan-chungtsiang.top

[S18] C：命令行参数
来源：http://yms.ywan-chungtsiang.top


<!-- 参考信息 -->