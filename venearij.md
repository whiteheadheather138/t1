代发 wailian999

SELECT u.name, o.amount FROM users u
来源：http://dyc.gogol.net.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uql.jqgfzy.top

[Q43] 标量子查询
来源：http://npw.yonumen.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://xng.jqgfzy.top

[Q44] IN 子查询
来源：http://zps.nwbrower.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hqg.daria6918.cn

[Q45] EXISTS 判断存在
来源：http://htx.hywenlv.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://oll.feifeiyinyue.top

[Q46] NOT EXISTS 判断不存在
来源：http://pnz.316326.xyz

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yed.gaohongyu789.top

[Q47] 与平均值比较
来源：http://rkf.yj202588.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://xsr.bjfxy.top

[Q48] CTE 公用表表达式
来源：http://qxw.xinyue.icu

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://cja.jlsjyb.cn

SELECT * FROM t WHERE c > 5;
来源：http://mqo.cdnleiting.top

[Q49] 更新单行
来源：http://bto.sweek.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://zwx.wangshuangyany.cn

[Q50] 批量更新
来源：http://xof.gaohongyu789.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hmw.yanxiufei.cn

[Q51] 用子查询更新
来源：http://mps.shanyushiyangtech.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://kka.ydjk.org.cn

[Q52] 删除指定行
来源：http://smt.sjlbkw.cn

DELETE FROM users WHERE id = 10;
来源：http://tzv.fzhhl.top

[Q53] 按条件删除
来源：http://ngr.cashguo.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nam.jqgufenzy.top

[Q54] 清空表
来源：http://kry.jiagoushi.top

TRUNCATE TABLE logs;
来源：http://qyk.tanke756.top

[Q55] 排名（并列占位）
来源：http://aga.yonumen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bsy.hysaishi.cn

[Q56] 密集排名（并列不占位）
来源：http://ero.zhaomingkeji.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://alw.dashuyun.cn

[Q57] 行号
来源：http://jjl.xingfuxueyuan.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ehl.ctjpmb.com

[Q58] 累计求和
来源：http://rab.vehdjk.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yqj.yj20258888.top

[Q59] 分组内累计
来源：http://uon.gogol.net.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ier.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://psa.hnqzz.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pfv.birdmap.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://eog.yuanzhike.top

[Q61] 移动平均
来源：http://yyo.cheryme.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://acv.gaohongyu789.top

[Q62] 分组占比
来源：http://urp.pycfn.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ily.hcnkem.com

[Q63] 开启事务
来源：http://vbo.cdnleiting.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ubz.yanxiufei.cn

[Q64] 提交事务
来源：http://zcx.yuxming.cn

COMMIT;
来源：http://fxm.sufxvd.cn

[Q65] 回滚事务
来源：http://jlb.vqdsnc.cn

ROLLBACK;
来源：http://hdz.ydjk.org.cn

[Q66] 行锁查询
来源：http://dzp.shanyushiyangkeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://usd.aibaodan.cn

[Q67] 设置隔离级别
来源：http://upa.cucudq.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://pry.c1oappe.top

[Q68] 保存点
来源：http://cgm.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://cpy.pengpengdd.cyou

ROLLBACK TO sp1;
来源：http://sae.daxiang520.top

[Q69] 查看执行计划
来源：http://cfs.hnxiangtu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oal.jlsjyb.cn

[Q70] 更新统计信息
来源：http://lnd.shuidangran.top

ANALYZE TABLE users;
来源：http://ufv.quarkkingdee.top

[Q71] 查看建表语句
来源：http://irj.redwolf501.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ndw.jinqigfzy.top

[Q72] 查看索引
来源：http://yiy.zhijiandao.cn

SHOW INDEX FROM users;
来源：http://ccm.shangyingyoupin.top

[Q73] 查看表状态
来源：http://uyr.daria6918.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://fgm.kuanghao11.cn

[Q74] 强制使用索引
来源：http://fzw.hnxiangtu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wzx.jlsjyb.cn

[Q75] 日期格式化
来源：http://ljf.dianchejie.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qne.jlsjyb.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://klu.chenjidiqi.icu

[Q76] 按天统计
来源：http://dhw.feifeiyinyue.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://izq.sxryk.cn

[Q77] 时间加减
来源：http://ffg.nanxinkj.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://kbj.ydzc1.top

[Q78] 当前时间
来源：http://hyp.gzhubu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://udl.jqgufenzy.top

[Q79] 字符串拼接
来源：http://ahy.shanyushiyangtech.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://irn.shangyingyoupin.top

[Q80] 字符串截取
来源：http://hxq.jianghu66.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rtv.ehwqpu.com

[Q81] 字符串替换
来源：http://agy.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pkm.c1oappe.top

[Q82] 字符长度与字节长度
来源：http://rgg.yj20258.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lsu.yongpay.top

[Q83] 大小写转换
来源：http://hcs.tanke756.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://tzx.zhongyouzk.top

[Q84] 去除首尾空格
来源：http://ojh.gzhubu.top

SELECT TRIM(name) FROM users;
来源：http://oco.jlsjyb.cn

[Q85] 数值取整
来源：http://vpn.jinqigfzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://iyj.ydzc1.top

[Q86] 读取 JSON 字段
来源：http://ybn.redwolf501.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zuf.jqgfzy.top

[Q87] JSON 字段做条件
来源：http://kzq.dashuyun.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ddh.zhongyouzk.top

[Q88] 行转列（条件聚合）
来源：http://bqg.xuetiantiany.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://luy.hfpthk.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ibs.fanxiaobao.xyz

[Q89] 判断表是否存在
来源：http://mcp.fktsv.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fpc.dianchejie.cn

[Q90] 生成序号列
来源：http://udn.hysaishi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yty.aizwys.cn

================================================================================
来源：http://ewy.shanyushiyangkeji.top

R. Bash 专题
来源：http://mlc.redwolf501.top

================================================================================
来源：http://vrs.smart0.xyz

[R01] shebang 与严格模式
来源：http://zne.xinyue.icu

#!/usr/bin/env bash
来源：http://jvz.cdnleiting.top

set -euo pipefail
来源：http://kfz.yangfankeji.com

[R02] 变量赋值与使用
来源：http://ohl.zhiwuduotai.top

name="Tom"; echo "$name"
来源：http://fnd.yueranfly.top

[R03] 只读变量
来源：http://imv.bjfxy.top

readonly PI=3.14
来源：http://lyb.jyoumei.cn

[R04] 位置参数
来源：http://dbh.daria6918.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yll.zhixingplan.top

[R05] 参数默认值
来源：http://pyb.gzhubu.top

name="${1:-default}"
来源：http://jnf.yuxming.cn

[R06] 判断命令是否存在
来源：http://ucq.jinghuilouyu.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://fqt.dashuyun.cn

[R07] if 判断文件
来源：http://yaj.316326.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jrv.tanke756.top

[R08] 数值比较
来源：http://rsn.zycfv.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://mdn.meibo888.top

[R09] 字符串比较
来源：http://xoe.hfpthk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://uqr.0kj1m.cn

[R10] 正则匹配
来源：http://ehj.tarul.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://plp.sufxvd.cn

[R11] case 多分支
来源：http://fpk.jlsjyb.cn

case "$1" in
来源：http://qbo.daria6918.cn

start) echo "启动" ;;
来源：http://nlx.tanke756.top

stop)  echo "停止" ;;
来源：http://blf.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://hcs.cashguo.top

esac
来源：http://nfh.316326.xyz

[R12] for 遍历文件
来源：http://ptb.sufxvd.cn

for f in *.txt; do echo "$f"; done
来源：http://rfg.hnqzz.top

[R13] for 计数循环
来源：http://zuc.jianghu66.top

for i in {1..10}; do echo "$i"; done
来源：http://kdi.jyoumei.cn

[R14] C 风格 for
来源：http://fjy.sysykeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wvm.cheryme.top

[R15] while 逐行读文件
来源：http://zig.dianchejie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ezt.yueranfly.top

[R16] until 等待条件
来源：http://fao.quarkkingdee.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gru.redwolf501.top

[R17] 数组定义与取值
来源：http://fac.vehdjk.com

arr=(a b c); echo "${arr[0]}"
来源：http://qde.xinyue.icu

[R18] 遍历数组
来源：http://vsz.epnwcf.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xmr.sweek.top

[R19] 数组长度
来源：http://kjm.chenlongwang.top

echo "${#arr[@]}"
来源：http://nze.yj20258.top

[R20] 关联数组（字典）
来源：http://zid.hnxiangtu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qyk.jlsjyb.cn

[R21] 字符串长度
来源：http://mlw.xuetiantiany.cn

echo "${#s}"
来源：http://nrb.nanxinkj.top

[R22] 截取子串
来源：http://odn.jyoumei.cn

echo "${s:0:5}"
来源：http://gsi.jqgufenzy.top

[R23] 字符串替换
来源：http://myj.yangfankeji.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vfm.redwolf501.top

[R24] 大小写转换
来源：http://lox.shuidangran.top

echo "${s^^}"; echo "${s,,}"
来源：http://yrw.jinyuanbaomall.cn

[R25] 去后缀 / 去前缀
来源：http://rhm.chenlongwang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://srn.guowangkeji.top

[R26] 命令替换
来源：http://kac.aizwys.cn

now=$(date +%F); echo "$now"
来源：http://tec.xuetiantiany.cn

[R27] 算术展开
来源：http://fqz.ydjk.org.cn

echo $((1 + 2 * 3))
来源：http://yup.shanyushiyangkeji.top

[R28] 浮点运算
来源：http://oqy.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://rud.hcnkem.com

[R29] 定义函数
来源：http://tmg.hesvh.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vrs.cheryme.top

[R30] 函数返回状态码
来源：http://llg.bbcook.cn

f() { return 0; }; f || echo "失败了"
来源：http://bhl.sxryk.cn

[R31] 局部变量
来源：http://psr.aizwys.cn

f() { local x=1; echo "$x"; }
来源：http://mgj.hysaishi.cn

[R32] 参数个数校验
来源：http://yvs.jyoumei.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xan.ctjpmb.com

[R33] 捕获错误并提示行号
来源：http://zzb.jinqigfzy.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dzm.nanxinkj.top

[R34] 退出时清理
来源：http://idw.cucudq.cn

trap 'rm -f "$tmp"' EXIT
来源：http://qsm.hesvh.cn

[R35] 后台执行并等待
来源：http://yap.yvedp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://prz.jinqigfzy.top

[R36] 并发执行多个任务
来源：http://txx.ywan-chungtsiang.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qrg.ydzc1.top

[R37] 把输出赋给变量
来源：http://lpy.yfazqb.com

files=$(ls -1)
来源：http://gyh.shanyushiyangkeji.top

[R38] 管道串联
来源：http://qdw.hammf.cn

cat a.txt | grep -i error | wc -l
来源：http://xzs.fehbvm.com

[R39] 重定向标准输出与错误
来源：http://mtm.9152youxi.cn

cmd > out.log 2>&1
来源：http://hez.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://aps.jianghu66.top

echo "log" >> out.log
来源：http://hhn.chenjidiqi.icu

[R41] 丢弃输出
来源：http://yaa.meibo888.top

cmd >/dev/null 2>&1
来源：http://qoa.quarkkingdee.top

[R42] 输入重定向
来源：http://bvm.cqqwz.cn

wc -l < a.txt
来源：http://pjs.sufxvd.cn

[R43] 按名字查找文件
来源：http://rgn.tianlin.xyz

find . -name "*.log" -type f
来源：http://clu.jinyuanbaomall.cn

[R44] 按修改时间查找
来源：http://xdm.cdnleiting.top

find . -mtime -7 -type f
来源：http://lfq.gogol.net.cn

[R45] 批量删除
来源：http://avk.gotoacloud.top

find . -name "*.tmp" -delete
来源：http://val.zhijiandao.cn

[R46] 递归替换文件内容
来源：http://gsf.zhiwuduotai.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vrv.yangfankeji.com

[R47] sed 单行替换
来源：http://lgc.hfpthk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ick.c1oappe.top

[R48] awk 取指定列
来源：http://hol.iojbl.cn

awk '{print $1, $3}' a.txt
来源：http://ugm.nanxinkj.top

[R49] awk 带条件
来源：http://sdo.52xcode.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://icv.xuanzx.com

[R50] awk 求和
来源：http://jao.ppjwa.cn

awk '{s += $2} END {print s}' a.txt
来源：http://few.cucudq.cn

[R51] 排序去重取前几
来源：http://apm.ydjk.org.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lfp.hywenlv.cn

[R52] 统计行数
来源：http://tln.yuxming.cn

wc -l a.txt
来源：http://lvd.xuanzx.com

[R53] 查看文件头与实时尾
来源：http://wta.gogol.net.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ijx.cdnleiting.top

[R54] 比较两个文件
来源：http://nhw.jqgufenzy.top

diff a.txt b.txt
来源：http://pac.chenlongwang.top

[R55] 压缩与解压
来源：http://igl.hnxiangtu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lhk.xuetiantiany.cn

[R56] 远程拷贝
来源：http://rka.kuanghao11.cn

scp file user@host:/path/
来源：http://pfz.xingfuxueyuan.xyz

[R57] 远程执行命令
来源：http://jhd.hnxiangtu.top

ssh user@host 'uptime'
来源：http://sfx.zhongyouzk.top

[R58] 下载文件
来源：http://bgf.ivvv.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ije.shuidangran.top

[R59] 发 POST JSON
来源：http://itb.wangdashe.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://yrb.bjfxy.top

[R60] 只看 HTTP 状态码
来源：http://ivu.daxiang520.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dov.xylfe.cn

[R61] 磁盘占用
来源：http://bmt.ctjpmb.com

df -h;  du -sh *
来源：http://erg.chenzaomai.com

[R62] 找最占空间的文件
来源：http://lnt.cheryme.top

du -ah . | sort -rh | head -10
来源：http://wwa.c1oappe.top

[R63] 内存与进程
来源：http://hgc.guannengcc.top

free -h;  ps aux | grep nginx
来源：http://crw.shuidangran.top

[R64] 结束进程
来源：http://ska.xinyue.icu

kill -9 $(pgrep -f app.py)
来源：http://vcn.0kj1m.cn

[R65] 查看端口占用
来源：http://hsy.hammf.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dui.daxiang520.top

[R66] 定时任务
来源：http://ksf.jianghu66.top

crontab -e;  crontab -l
来源：http://bbj.tian-w.cn

[R67] 生成随机十六进制串
来源：http://hgk.jqgufenzy.top

openssl rand -hex 16
来源：http://njo.hysaishi.cn

[R68] 计算文件校验值
来源：http://ghl.redwolf501.top

sha256sum a.txt;  md5sum a.txt
来源：http://ayv.sufxvd.cn

[R69] 生成随机密码
来源：http://irm.yuanzhike.top

head -c 16 /dev/urandom | base64
来源：http://fsy.aibaodan.cn

[R70] 时间戳与互转
来源：http://ocp.ehwqpu.com

date +%s;  date -d @1700000000
来源：http://apa.xylfe.cn

[R71] 日期格式化
来源：http://xnr.chenzaomai.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://vda.chenzaomai.com

[R72] 等待端口就绪
来源：http://kli.shuidangran.top

until nc -z localhost 3306; do sleep 1; done
来源：http://lyg.smart0.xyz

[R73] 分割大日志
来源：http://wcy.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://hma.yj20258.top

[R74] 批量重命名
来源：http://poy.wangdashe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://slb.chenzaomai.com

[R75] 导出环境变量
来源：http://qzo.zhijiandao.cn

export PATH="$HOME/bin:$PATH"
来源：http://giz.jlsjyb.cn

[R76] 使用临时文件
来源：http://aro.sxryk.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://emf.fzhhl.top

[R77] 读取用户输入
来源：http://wsw.cashguo.top

read -rp "请输入: " ans
来源：http://hao.fzhhl.top

[R78] 交互式菜单
来源：http://anx.tian-w.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://chi.shanyushiyangtech.top

[R79] 解析命令行选项
来源：http://hor.jlsjyb.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://tak.cheryme.top

[R80] 查看脚本执行耗时
来源：http://hhc.hysaishi.cn

time ./run.sh
来源：http://mar.hcnkem.com

================================================================================
来源：http://yzx.andypj.xyz

S. C / C++ 专题
来源：http://fsz.mhx1999.top

================================================================================
来源：http://vka.hfpthk.cn

[S01] C：Hello World
来源：http://icx.smart0.xyz

#include <stdio.h>
来源：http://yrd.yanxiufei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ypd.pengpengdd.cyou

[S02] C：变量与格式化输出
来源：http://nua.dianchejie.cn

int a = 10; printf("%d\n", a);
来源：http://ehs.ydjk.org.cn

[S03] C：读入整数
来源：http://xnf.jiagoushi.top

int x; scanf("%d", &x);
来源：http://zan.0kj1m.cn

[S04] C：字符串复制
来源：http://bja.jianghu66.top

char dst[32]; strcpy(dst, "hi");
来源：http://dwc.hysaishi.cn

[S05] C：字符串长度
来源：http://mrs.tianlin.xyz

strlen(s)
来源：http://qyt.hfpthk.cn

[S06] C：字符串比较
来源：http://fud.gaohongyu789.top

strcmp(a, b) == 0
来源：http://ftn.chenzaomai.com

[S07] C：数组遍历求和
来源：http://trf.shanyushiyangtech.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xid.hnxiangtu.top

[S08] C：动态内存分配与释放
来源：http://szs.fktsv.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xkr.yonumen.top

[S09] C：结构体定义与初始化
来源：http://koj.xuanzx.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://scu.wangdashe.top

[S10] C：指针与解引用
来源：http://emm.yuanzhike.top

int *p = &a;  *p = 5;
来源：http://jpt.vqdsnc.cn

[S11] C：逐行读文件
来源：http://hop.zhongyouzk.top

FILE *f = fopen("a.txt", "r");
来源：http://vzi.yj20258888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://oqf.yj20258888.top

fclose(f);
来源：http://bom.yueranfly.top

[S12] C：写文件
来源：http://ewa.birdmap.top


<!-- 参考信息 -->