代发 wailian999

[Q36] 左连接
来源：http://xmu.dianchejie.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://qfa.guannengcc.top

[Q37] 右连接
来源：http://hcj.hnqzz.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://vsn.zhixingplan.top

[Q38] 全外连接（PostgreSQL）
来源：http://gzz.zdbjq.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://qnh.pycfn.com

[Q39] 自连接（查上下级）
来源：http://meq.jqgufenzy.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://hfx.yueranfly.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qbg.chenjidiqi.icu

[Q40] 交叉连接（笛卡尔积）
来源：http://oak.dashuyun.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ssg.xuanzx.com

[Q41] 多表连接
来源：http://wjc.zhijiandao.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://uqd.xinyue.icu

JOIN users u ON u.id = o.user_id
来源：http://nue.hammf.cn

JOIN products p ON p.id = o.product_id;
来源：http://weh.ywan-chungtsiang.top

[Q42] 连接条件附加过滤
来源：http://pbv.xuanzx.com

SELECT u.name, o.amount FROM users u
来源：http://toe.zhengqikj.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://lgd.iojbl.cn

[Q43] 标量子查询
来源：http://ine.yj20258.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://eca.shangyingyoupin.top

[Q44] IN 子查询
来源：http://lwg.xingfuxueyuan.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://xsa.yuanzhike.top

[Q45] EXISTS 判断存在
来源：http://jtk.sweek.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://ybw.yj202588.top

[Q46] NOT EXISTS 判断不存在
来源：http://gxo.bjfxy.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blc.cqqwz.cn

[Q47] 与平均值比较
来源：http://unn.fanxiaobao.xyz

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://vvw.xuanzx.com

[Q48] CTE 公用表表达式
来源：http://nid.shanyushiyangkeji.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ymt.epnwcf.com

SELECT * FROM t WHERE c > 5;
来源：http://fgk.dianchejie.cn

[Q49] 更新单行
来源：http://zai.yj20258888.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://uej.ppjwa.cn

[Q50] 批量更新
来源：http://xgb.sxryk.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://qmw.fanxiaobao.xyz

[Q51] 用子查询更新
来源：http://rcg.zdbjq.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hqs.fzhhl.top

[Q52] 删除指定行
来源：http://ldl.pycfn.com

DELETE FROM users WHERE id = 10;
来源：http://tmk.tarul.cn

[Q53] 按条件删除
来源：http://ewk.yj20258888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fsd.kuanghao11.cn

[Q54] 清空表
来源：http://lwl.zdqjudy.top

TRUNCATE TABLE logs;
来源：http://hut.sjlbkw.cn

[Q55] 排名（并列占位）
来源：http://kmp.c1oappe.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tjb.svipenyu.cn

[Q56] 密集排名（并列不占位）
来源：http://obg.xinyue.icu

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://toa.316326.xyz

[Q57] 行号
来源：http://djx.redwolf501.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hvx.cucudq.cn

[Q58] 累计求和
来源：http://kkh.ivvv.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://qcv.svipenyu.cn

[Q59] 分组内累计
来源：http://mrk.zdqjudy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://elb.zycfv.cn

[Q60] 取上一行 / 下一行
来源：http://mne.ivvv.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ebt.xuetiantiany.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://awt.sysykeji.top

[Q61] 移动平均
来源：http://zpy.snrcjt.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://iir.c1oappe.top

[Q62] 分组占比
来源：http://ere.nanxinkj.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jsv.hysaishi.cn

[Q63] 开启事务
来源：http://kiq.zhoulong.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://tma.guowangkeji.top

[Q64] 提交事务
来源：http://pwo.zdqjudy.top

COMMIT;
来源：http://xtk.guannengcc.top

[Q65] 回滚事务
来源：http://pex.fehbvm.com

ROLLBACK;
来源：http://ttm.xinyue.icu

[Q66] 行锁查询
来源：http://uho.tian-w.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cao.ehwqpu.com

[Q67] 设置隔离级别
来源：http://rus.hongshengwenyu.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://uoh.bbcook.cn

[Q68] 保存点
来源：http://htp.fehbvm.com

SAVEPOINT sp1;
来源：http://yow.yangfankeji.com

ROLLBACK TO sp1;
来源：http://hvr.birdmap.top

[Q69] 查看执行计划
来源：http://gqb.cqqwz.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fra.haohaochexian.top

[Q70] 更新统计信息
来源：http://sog.xuetiantiany.cn

ANALYZE TABLE users;
来源：http://qsi.redwolf501.top

[Q71] 查看建表语句
来源：http://pwm.jyoumei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ujj.pycfn.com

[Q72] 查看索引
来源：http://vtf.gotoacloud.top

SHOW INDEX FROM users;
来源：http://eec.jinqigufen.top

[Q73] 查看表状态
来源：http://oyy.yfazqb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://amu.yanxiufei.cn

[Q74] 强制使用索引
来源：http://mml.0kj1m.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xwm.haohaochexian.top

[Q75] 日期格式化
来源：http://rpm.ctjpmb.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pyv.xuanzx.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://diq.tarul.cn

[Q76] 按天统计
来源：http://rsp.sxryk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nfq.hcnkem.com

[Q77] 时间加减
来源：http://spm.jqgfzy.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zfx.yonumen.top

[Q78] 当前时间
来源：http://klq.tianlin.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://yzw.yueranfly.top

[Q79] 字符串拼接
来源：http://kka.wangshuangyany.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://idt.tianlin.xyz

[Q80] 字符串截取
来源：http://phr.jqgfzy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zsu.aibaodan.cn

[Q81] 字符串替换
来源：http://joj.jiagoushi.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://uht.haohaochexian.top

[Q82] 字符长度与字节长度
来源：http://vdc.c1oappe.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fqm.hongshengwenyu.top

[Q83] 大小写转换
来源：http://hax.haohaochexian.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ank.gaohongyu789.top

[Q84] 去除首尾空格
来源：http://zhv.hnqzz.top

SELECT TRIM(name) FROM users;
来源：http://wfh.shangyingyoupin.top

[Q85] 数值取整
来源：http://tdw.nanxuanxn.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tqw.jlsjyb.cn

[Q86] 读取 JSON 字段
来源：http://pvg.zhoulong.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://yrm.vqdsnc.cn

[Q87] JSON 字段做条件
来源：http://rtc.vehdjk.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pxa.ctjpmb.com

[Q88] 行转列（条件聚合）
来源：http://wzj.daxiang520.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ksw.chenlongwang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://fem.vqdsnc.cn

[Q89] 判断表是否存在
来源：http://rtf.cucudq.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vho.gaohongyu789.top

[Q90] 生成序号列
来源：http://kbz.xylfe.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dbi.yuxming.cn

================================================================================
来源：http://nfo.fzhhl.top

R. Bash 专题
来源：http://ded.52xcode.cn

================================================================================
来源：http://vta.gotoacloud.top

[R01] shebang 与严格模式
来源：http://tch.tian-w.cn

#!/usr/bin/env bash
来源：http://hfx.jinyuanbaomall.cn

set -euo pipefail
来源：http://abe.tarul.cn

[R02] 变量赋值与使用
来源：http://mck.cheryme.top

name="Tom"; echo "$name"
来源：http://wwg.zycfv.cn

[R03] 只读变量
来源：http://ncr.birdmap.top

readonly PI=3.14
来源：http://aoc.guowangkeji.top

[R04] 位置参数
来源：http://kol.zhoulong.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wqx.ehwqpu.com

[R05] 参数默认值
来源：http://gnr.hesvh.cn

name="${1:-default}"
来源：http://fbn.xziqi.cn

[R06] 判断命令是否存在
来源：http://vmb.shuidangran.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vzi.gaohongyu789.top

[R07] if 判断文件
来源：http://red.wangshuangyany.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wma.uphjek.com

[R08] 数值比较
来源：http://fmc.svipenyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://fex.fzhhl.top

[R09] 字符串比较
来源：http://zin.hnqzz.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vrk.daxiang520.top

[R10] 正则匹配
来源：http://nhq.gaohongyu789.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mrx.nanxuanxn.top

[R11] case 多分支
来源：http://ujr.zhengqikj.top

case "$1" in
来源：http://sjf.redwolf501.top

start) echo "启动" ;;
来源：http://qak.dianchejie.cn

stop)  echo "停止" ;;
来源：http://dpw.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://uov.dianchejie.cn

esac
来源：http://hwi.ctjpmb.com

[R12] for 遍历文件
来源：http://vxs.gzhubu.top

for f in *.txt; do echo "$f"; done
来源：http://mny.jyoumei.cn

[R13] for 计数循环
来源：http://ira.guowangkeji.top

for i in {1..10}; do echo "$i"; done
来源：http://uwv.pengpengdd.cyou

[R14] C 风格 for
来源：http://qne.hesvh.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ama.meibo888.top

[R15] while 逐行读文件
来源：http://kwk.zhixingplan.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://amc.jinqigfzy.top

[R16] until 等待条件
来源：http://rfg.redwolf501.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://psk.fehbvm.com

[R17] 数组定义与取值
来源：http://olm.chenlongwang.top

arr=(a b c); echo "${arr[0]}"
来源：http://kia.fanxiaobao.xyz

[R18] 遍历数组
来源：http://qyf.ehwqpu.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pau.zhixingplan.top

[R19] 数组长度
来源：http://sbl.zdqjudy.top

echo "${#arr[@]}"
来源：http://utz.shanyushiyangtech.top

[R20] 关联数组（字典）
来源：http://edi.svipenyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gjp.zhongyouzk.top

[R21] 字符串长度
来源：http://vql.xuetiantiany.cn

echo "${#s}"
来源：http://dwb.shuidangran.top

[R22] 截取子串
来源：http://lfq.hcnkem.com

echo "${s:0:5}"
来源：http://mfi.zhijiandao.cn

[R23] 字符串替换
来源：http://epq.sweek.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kns.hywenlv.cn

[R24] 大小写转换
来源：http://gub.iojbl.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xfm.ppjwa.cn

[R25] 去后缀 / 去前缀
来源：http://dil.dashuyun.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://blw.vehdjk.com

[R26] 命令替换
来源：http://ogq.birdmap.top

now=$(date +%F); echo "$now"
来源：http://ypo.ppjwa.cn

[R27] 算术展开
来源：http://zwf.jyoumei.cn

echo $((1 + 2 * 3))
来源：http://gml.guannengcc.top

[R28] 浮点运算
来源：http://cbb.xuanzx.com

echo "scale=2; 10/3" | bc
来源：http://gtb.ybcxt.top

[R29] 定义函数
来源：http://eok.yuxming.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wrv.nwbrower.top

[R30] 函数返回状态码
来源：http://hbx.hammf.cn

f() { return 0; }; f || echo "失败了"
来源：http://vkj.yj20258.top

[R31] 局部变量
来源：http://vke.dianchejie.cn

f() { local x=1; echo "$x"; }
来源：http://svl.mhx1999.top

[R32] 参数个数校验
来源：http://wvf.gotoacloud.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zbw.xingfuxueyuan.xyz

[R33] 捕获错误并提示行号
来源：http://xzg.yj20258888.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hii.zhaomingkeji.xyz

[R34] 退出时清理
来源：http://uxm.sjlbkw.cn

trap 'rm -f "$tmp"' EXIT
来源：http://abx.kuanghao11.cn

[R35] 后台执行并等待
来源：http://bse.9152youxi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oum.vqdsnc.cn

[R36] 并发执行多个任务
来源：http://sio.sweek.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://klc.mhx1999.top

[R37] 把输出赋给变量
来源：http://hnx.jyoumei.cn

files=$(ls -1)
来源：http://jma.chenzaomai.com

[R38] 管道串联
来源：http://ytr.haohaochexian.top

cat a.txt | grep -i error | wc -l
来源：http://rey.fzhhl.top

[R39] 重定向标准输出与错误
来源：http://tow.gotoacloud.top

cmd > out.log 2>&1
来源：http://gne.c1oappe.top

[R40] 追加写日志
来源：http://icu.iojbl.cn

echo "log" >> out.log
来源：http://rtb.c1oappe.top

[R41] 丢弃输出
来源：http://gaa.yuanzhike.top

cmd >/dev/null 2>&1
来源：http://ldr.yanxiufei.cn

[R42] 输入重定向
来源：http://jww.ppjwa.cn

wc -l < a.txt
来源：http://xzf.nanxinkj.top

[R43] 按名字查找文件
来源：http://qdf.ivvv.top

find . -name "*.log" -type f
来源：http://eid.wangdashe.top

[R44] 按修改时间查找
来源：http://tbs.guowangkeji.top

find . -mtime -7 -type f
来源：http://ekx.jiagoushi.top

[R45] 批量删除
来源：http://cqh.wangdashe.top

find . -name "*.tmp" -delete
来源：http://rzj.zycfv.cn

[R46] 递归替换文件内容
来源：http://yrw.daxiang520.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nik.sjlbkw.cn

[R47] sed 单行替换
来源：http://fvn.zycfv.cn

sed -i 's/foo/bar/g' a.txt
来源：http://wgu.yfazqb.com

[R48] awk 取指定列
来源：http://ryy.yueranfly.top

awk '{print $1, $3}' a.txt
来源：http://jrq.cdnleiting.top

[R49] awk 带条件
来源：http://rrb.jlsjyb.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kol.yj202588.top

[R50] awk 求和
来源：http://fzr.daxiang520.top

awk '{s += $2} END {print s}' a.txt
来源：http://lnl.guowangkeji.top

[R51] 排序去重取前几
来源：http://ivy.yfazqb.com

sort a.txt | uniq -c | sort -rn | head
来源：http://eju.quarkkingdee.top

[R52] 统计行数
来源：http://hag.kuanghao11.cn

wc -l a.txt
来源：http://eom.316326.xyz

[R53] 查看文件头与实时尾
来源：http://tsx.chenjidiqi.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ucd.ywan-chungtsiang.top

[R54] 比较两个文件
来源：http://wkg.hysaishi.cn

diff a.txt b.txt
来源：http://xkk.pengpengdd.cyou

[R55] 压缩与解压
来源：http://dxi.ybcxt.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vgj.chenjidiqi.icu

[R56] 远程拷贝
来源：http://yec.9152youxi.cn

scp file user@host:/path/
来源：http://rjo.ivvv.top

[R57] 远程执行命令
来源：http://fvc.dianchejie.cn

ssh user@host 'uptime'
来源：http://auu.pengpengdd.cyou

[R58] 下载文件
来源：http://kmn.sxryk.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hva.zdqjudy.top

[R59] 发 POST JSON
来源：http://edf.andypj.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://akf.yanxiufei.cn

[R60] 只看 HTTP 状态码
来源：http://rod.zhixingplan.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zbv.feifeiyinyue.top

[R61] 磁盘占用
来源：http://hvg.zhijiandao.cn

df -h;  du -sh *
来源：http://lyd.uphjek.com

[R62] 找最占空间的文件
来源：http://mqt.zhoulong.xyz

du -ah . | sort -rh | head -10
来源：http://tqk.jianghu66.top

[R63] 内存与进程
来源：http://zfp.gogol.net.cn

free -h;  ps aux | grep nginx
来源：http://rjd.iojbl.cn

[R64] 结束进程
来源：http://ezy.tian-w.cn

kill -9 $(pgrep -f app.py)
来源：http://dwc.snrcjt.cn

[R65] 查看端口占用
来源：http://uyo.zdqjudy.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uou.shzxlz.cn

[R66] 定时任务
来源：http://ptm.xingfuxueyuan.xyz

crontab -e;  crontab -l
来源：http://wdq.wangdashe.top

[R67] 生成随机十六进制串
来源：http://idi.havefunace.top

openssl rand -hex 16
来源：http://qmt.ivvv.top

[R68] 计算文件校验值
来源：http://djq.aizwys.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tfh.nanxinkj.top

[R69] 生成随机密码
来源：http://dks.hfpthk.cn

head -c 16 /dev/urandom | base64
来源：http://ouu.haohaochexian.top

[R70] 时间戳与互转
来源：http://tua.daxiang520.top

date +%s;  date -d @1700000000
来源：http://xcx.jiagoushi.top

[R71] 日期格式化
来源：http://ozb.xuanzx.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://dze.zdqjudy.top

[R72] 等待端口就绪
来源：http://hty.chenjidiqi.icu

until nc -z localhost 3306; do sleep 1; done
来源：http://rsg.tanke756.top

[R73] 分割大日志
来源：http://xsa.yj202588.top

split -l 1000 big.log part_
来源：http://ojh.svipenyu.cn

[R74] 批量重命名
来源：http://xsy.xylfe.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hpw.chenlongwang.top

[R75] 导出环境变量
来源：http://agn.shanyushiyangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://fsi.nanxinkj.top

[R76] 使用临时文件
来源：http://asw.xuetiantiany.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lkm.xylfe.cn

[R77] 读取用户输入
来源：http://gyf.epnwcf.com

read -rp "请输入: " ans
来源：http://kqg.daxiang520.top

[R78] 交互式菜单
来源：http://xxk.zhaomingkeji.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://pgy.hongshengwenyu.top

[R79] 解析命令行选项
来源：http://ehg.meibo888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ruu.jlsjyb.cn

[R80] 查看脚本执行耗时
来源：http://yji.yj20258.top

time ./run.sh
来源：http://kjx.andypj.xyz

================================================================================
来源：http://jyg.uphjek.com

S. C / C++ 专题
来源：http://hwr.hysaishi.cn

================================================================================
来源：http://erp.sysykeji.top

[S01] C：Hello World
来源：http://avl.yj20258888.top

#include <stdio.h>
来源：http://lvl.yanxiufei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://veg.shzxlz.cn

[S02] C：变量与格式化输出
来源：http://zal.yanxiufei.cn

int a = 10; printf("%d\n", a);
来源：http://wrz.ctjpmb.com

[S03] C：读入整数
来源：http://yak.yueranfly.top

int x; scanf("%d", &x);
来源：http://zck.iojbl.cn

[S04] C：字符串复制
来源：http://jps.andypj.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://smc.tian-w.cn

[S05] C：字符串长度
来源：http://wwc.jqgufenzy.top


<!-- 参考信息 -->