代发 wailian999

[Q36] 左连接
来源：http://zug.xingfuxueyuan.xyz

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mbe.c1oappe.top

[Q37] 右连接
来源：http://zqz.hysaishi.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://apc.jqgfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://lwx.ppjwa.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ste.yanxiufei.cn

[Q39] 自连接（查上下级）
来源：http://kke.chenlongwang.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://tqd.52xcode.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ixw.jlsjyb.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://sqq.hnqzz.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hsq.aizwys.cn

[Q41] 多表连接
来源：http://pgk.zhijiandao.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://jfm.tarul.cn

JOIN users u ON u.id = o.user_id
来源：http://ois.zhiwuduotai.top

JOIN products p ON p.id = o.product_id;
来源：http://vfg.hysaishi.cn

[Q42] 连接条件附加过滤
来源：http://vvf.gotoacloud.top

SELECT u.name, o.amount FROM users u
来源：http://ajx.yj202588.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://erv.xingfuxueyuan.xyz

[Q43] 标量子查询
来源：http://jjq.shuidangran.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://rpo.iojbl.cn

[Q44] IN 子查询
来源：http://tvs.tianlin.xyz

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mcp.cucudq.cn

[Q45] EXISTS 判断存在
来源：http://leq.0kj1m.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mjg.haohaochexian.top

[Q46] NOT EXISTS 判断不存在
来源：http://tsn.hammf.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://pxy.guowangkeji.top

[Q47] 与平均值比较
来源：http://lql.aibaodan.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://brj.9152youxi.cn

[Q48] CTE 公用表表达式
来源：http://cnj.hnxiangtu.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qnv.pengpengdd.cyou

SELECT * FROM t WHERE c > 5;
来源：http://etj.xylfe.cn

[Q49] 更新单行
来源：http://neg.shuidangran.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ugo.birdmap.top

[Q50] 批量更新
来源：http://yvc.gotoacloud.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://dab.mhx1999.top

[Q51] 用子查询更新
来源：http://rzs.tian-w.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oxc.ybcxt.top

[Q52] 删除指定行
来源：http://mbe.yvedp.cn

DELETE FROM users WHERE id = 10;
来源：http://lzb.ydjk.org.cn

[Q53] 按条件删除
来源：http://aii.hywenlv.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://xru.zhoulong.xyz

[Q54] 清空表
来源：http://feq.aibaodan.cn

TRUNCATE TABLE logs;
来源：http://qcy.ctjpmb.com

[Q55] 排名（并列占位）
来源：http://tqu.epnwcf.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://try.yongpay.top

[Q56] 密集排名（并列不占位）
来源：http://qme.feifeiyinyue.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://jpq.ppjwa.cn

[Q57] 行号
来源：http://jym.yongpay.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ccm.vqdsnc.cn

[Q58] 累计求和
来源：http://mjk.jiagoushi.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://taf.yj20258.top

[Q59] 分组内累计
来源：http://vqm.jiagoushi.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://etn.zycfv.cn

[Q60] 取上一行 / 下一行
来源：http://tqi.zycfv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uvo.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://qyl.ehwqpu.com

[Q61] 移动平均
来源：http://xpw.birdmap.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://efw.shanyushiyangtech.top

[Q62] 分组占比
来源：http://ttv.andypj.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jti.chenzaomai.com

[Q63] 开启事务
来源：http://yjs.yfazqb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://kna.yonumen.top

[Q64] 提交事务
来源：http://ehs.fktsv.cn

COMMIT;
来源：http://tyt.cucudq.cn

[Q65] 回滚事务
来源：http://nvd.wangdashe.top

ROLLBACK;
来源：http://ovw.hnqzz.top

[Q66] 行锁查询
来源：http://six.xuetiantiany.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://zie.0kj1m.cn

[Q67] 设置隔离级别
来源：http://rtu.pycfn.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://awd.hnqzz.top

[Q68] 保存点
来源：http://uyv.zhaomingkeji.xyz

SAVEPOINT sp1;
来源：http://zbp.dashuyun.cn

ROLLBACK TO sp1;
来源：http://cyw.yfazqb.com

[Q69] 查看执行计划
来源：http://knv.sysykeji.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qtq.chenjidiqi.icu

[Q70] 更新统计信息
来源：http://qlf.vqdsnc.cn

ANALYZE TABLE users;
来源：http://qqw.tanke756.top

[Q71] 查看建表语句
来源：http://qzh.hesvh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vns.sweek.top

[Q72] 查看索引
来源：http://xxb.fehbvm.com

SHOW INDEX FROM users;
来源：http://iud.yj202588.top

[Q73] 查看表状态
来源：http://jps.pycfn.com

SHOW TABLE STATUS LIKE 'users';
来源：http://otv.ehwqpu.com

[Q74] 强制使用索引
来源：http://mxv.jlsjyb.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dsr.aizwys.cn

[Q75] 日期格式化
来源：http://bub.cdnleiting.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ayf.shzxlz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rxm.hfpthk.cn

[Q76] 按天统计
来源：http://ljc.pengpengdd.cyou

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://iyv.ehwqpu.com

[Q77] 时间加减
来源：http://gdc.hesvh.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cme.cdnleiting.top

[Q78] 当前时间
来源：http://rfa.cashguo.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sjp.daria6918.cn

[Q79] 字符串拼接
来源：http://htu.daria6918.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rzt.smart0.xyz

[Q80] 字符串截取
来源：http://tig.zhijiandao.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bww.xinyue.icu

[Q81] 字符串替换
来源：http://lge.fanxiaobao.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://nea.jinghuilouyu.cn

[Q82] 字符长度与字节长度
来源：http://bih.ydjk.org.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://bnb.jqgufenzy.top

[Q83] 大小写转换
来源：http://tga.xuetiantiany.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dly.ivvv.top

[Q84] 去除首尾空格
来源：http://kxi.hammf.cn

SELECT TRIM(name) FROM users;
来源：http://jnd.hnxiangtu.top

[Q85] 数值取整
来源：http://byj.yonumen.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://bru.tian-w.cn

[Q86] 读取 JSON 字段
来源：http://ewu.316326.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://asi.zhaomingkeji.xyz

[Q87] JSON 字段做条件
来源：http://ivz.daria6918.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ydd.snrcjt.cn

[Q88] 行转列（条件聚合）
来源：http://fzj.cheryme.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gyn.jqgfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xab.birdmap.top

[Q89] 判断表是否存在
来源：http://ley.bbcook.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wmu.bjfxy.top

[Q90] 生成序号列
来源：http://spx.gzhubu.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ipw.cdnleiting.top

================================================================================
来源：http://poh.hnqzz.top

R. Bash 专题
来源：http://hki.jianghu66.top

================================================================================
来源：http://tpb.zhaomingkeji.xyz

[R01] shebang 与严格模式
来源：http://sqr.guannengcc.top

#!/usr/bin/env bash
来源：http://lym.jiagoushi.top

set -euo pipefail
来源：http://smu.ydjk.org.cn

[R02] 变量赋值与使用
来源：http://tgy.shanyushiyangkeji.top

name="Tom"; echo "$name"
来源：http://wuw.quarkkingdee.top

[R03] 只读变量
来源：http://rrr.gotoacloud.top

readonly PI=3.14
来源：http://rxe.hywenlv.cn

[R04] 位置参数
来源：http://vxj.ctjpmb.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://twj.birdmap.top

[R05] 参数默认值
来源：http://jht.nanxuanxn.top

name="${1:-default}"
来源：http://ojr.cheryme.top

[R06] 判断命令是否存在
来源：http://hrr.zhixingplan.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://daq.svipenyu.cn

[R07] if 判断文件
来源：http://eug.xinyue.icu

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tny.tarul.cn

[R08] 数值比较
来源：http://pua.jinyuanbaomall.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wac.jlsjyb.cn

[R09] 字符串比较
来源：http://gmt.aizwys.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bku.zdbjq.cn

[R10] 正则匹配
来源：http://jjd.shangyingyoupin.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wkp.zdbjq.cn

[R11] case 多分支
来源：http://ccf.sysykeji.top

case "$1" in
来源：http://yhp.sweek.top

start) echo "启动" ;;
来源：http://rdq.zhixingplan.top

stop)  echo "停止" ;;
来源：http://bri.hysaishi.cn

*)     echo "未知命令" ;;
来源：http://seg.aizwys.cn

esac
来源：http://fhd.sweek.top

[R12] for 遍历文件
来源：http://esz.svipenyu.cn

for f in *.txt; do echo "$f"; done
来源：http://jiw.shzxlz.cn

[R13] for 计数循环
来源：http://rpl.dashuyun.cn

for i in {1..10}; do echo "$i"; done
来源：http://xco.ctjpmb.com

[R14] C 风格 for
来源：http://dms.shuidangran.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vtc.tanke756.top

[R15] while 逐行读文件
来源：http://nrh.bjfxy.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zyx.ppjwa.cn

[R16] until 等待条件
来源：http://xht.svipenyu.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://zyb.gaohongyu789.top

[R17] 数组定义与取值
来源：http://jyp.yfazqb.com

arr=(a b c); echo "${arr[0]}"
来源：http://uxb.yuxming.cn

[R18] 遍历数组
来源：http://qur.hnqzz.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://bru.hammf.cn

[R19] 数组长度
来源：http://jfw.jinghuilouyu.cn

echo "${#arr[@]}"
来源：http://hlc.yuanzhike.top

[R20] 关联数组（字典）
来源：http://pns.gotoacloud.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kiw.hesvh.cn

[R21] 字符串长度
来源：http://vmg.cucudq.cn

echo "${#s}"
来源：http://nbk.shuidangran.top

[R22] 截取子串
来源：http://htg.vehdjk.com

echo "${s:0:5}"
来源：http://dba.vehdjk.com

[R23] 字符串替换
来源：http://pid.sufxvd.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ard.pycfn.com

[R24] 大小写转换
来源：http://ouj.yongpay.top

echo "${s^^}"; echo "${s,,}"
来源：http://fcr.haohaochexian.top

[R25] 去后缀 / 去前缀
来源：http://wot.bbcook.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pqh.zycfv.cn

[R26] 命令替换
来源：http://tod.nanxuanxn.top

now=$(date +%F); echo "$now"
来源：http://rcf.andypj.xyz

[R27] 算术展开
来源：http://ejl.daxiang520.top

echo $((1 + 2 * 3))
来源：http://fgq.c1oappe.top

[R28] 浮点运算
来源：http://ley.birdmap.top

echo "scale=2; 10/3" | bc
来源：http://tlf.mhx1999.top

[R29] 定义函数
来源：http://gdn.uphjek.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://abe.hfpthk.cn

[R30] 函数返回状态码
来源：http://jrn.zhengqikj.top

f() { return 0; }; f || echo "失败了"
来源：http://pnb.hammf.cn

[R31] 局部变量
来源：http://rbx.xinyue.icu

f() { local x=1; echo "$x"; }
来源：http://rut.dianchejie.cn

[R32] 参数个数校验
来源：http://ntd.haohaochexian.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://act.ppjwa.cn

[R33] 捕获错误并提示行号
来源：http://yis.hnxiangtu.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yca.0kj1m.cn

[R34] 退出时清理
来源：http://ltf.zdqjudy.top

trap 'rm -f "$tmp"' EXIT
来源：http://kdn.zhijiandao.cn

[R35] 后台执行并等待
来源：http://rjb.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://qhw.jianghu66.top

[R36] 并发执行多个任务
来源：http://vir.guowangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hbf.tian-w.cn

[R37] 把输出赋给变量
来源：http://gxf.dianchejie.cn

files=$(ls -1)
来源：http://tot.ydjk.org.cn

[R38] 管道串联
来源：http://ibw.316326.xyz

cat a.txt | grep -i error | wc -l
来源：http://yir.gaohongyu789.top

[R39] 重定向标准输出与错误
来源：http://iyy.yvedp.cn

cmd > out.log 2>&1
来源：http://pyz.uphjek.com

[R40] 追加写日志
来源：http://zws.9152youxi.cn

echo "log" >> out.log
来源：http://zjp.c1oappe.top

[R41] 丢弃输出
来源：http://rgd.sjlbkw.cn

cmd >/dev/null 2>&1
来源：http://bff.pycfn.com

[R42] 输入重定向
来源：http://bhs.xuanzx.com

wc -l < a.txt
来源：http://nxh.cashguo.top

[R43] 按名字查找文件
来源：http://tpe.yanxiufei.cn

find . -name "*.log" -type f
来源：http://jti.hysaishi.cn

[R44] 按修改时间查找
来源：http://mie.jlsjyb.cn

find . -mtime -7 -type f
来源：http://tqd.nanxuanxn.top

[R45] 批量删除
来源：http://hib.xinyue.icu

find . -name "*.tmp" -delete
来源：http://wks.andypj.xyz

[R46] 递归替换文件内容
来源：http://ufg.dianchejie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://pmx.nwbrower.top

[R47] sed 单行替换
来源：http://xys.ivvv.top

sed -i 's/foo/bar/g' a.txt
来源：http://kvv.zhaomingkeji.xyz

[R48] awk 取指定列
来源：http://wez.zhongyouzk.top

awk '{print $1, $3}' a.txt
来源：http://fsu.yuxming.cn

[R49] awk 带条件
来源：http://rzg.hysaishi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ioo.316326.xyz

[R50] awk 求和
来源：http://ive.shanyushiyangtech.top

awk '{s += $2} END {print s}' a.txt
来源：http://aov.pengpengdd.cyou

[R51] 排序去重取前几
来源：http://zct.fanxiaobao.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://myg.daria6918.cn

[R52] 统计行数
来源：http://xkk.zhengqikj.top

wc -l a.txt
来源：http://off.nanxuanxn.top

[R53] 查看文件头与实时尾
来源：http://tzk.daria6918.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xwc.nanxinkj.top

[R54] 比较两个文件
来源：http://jjm.chenzaomai.com

diff a.txt b.txt
来源：http://bba.pycfn.com

[R55] 压缩与解压
来源：http://obb.tian-w.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dju.zhengqikj.top

[R56] 远程拷贝
来源：http://sql.hnxiangtu.top

scp file user@host:/path/
来源：http://tdr.daxiang520.top

[R57] 远程执行命令
来源：http://cgx.jyoumei.cn

ssh user@host 'uptime'
来源：http://kjn.pengpengdd.cyou

[R58] 下载文件
来源：http://jiy.cucudq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kvt.zhoulong.xyz

[R59] 发 POST JSON
来源：http://mwq.daxiang520.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rpk.sysykeji.top

[R60] 只看 HTTP 状态码
来源：http://fiu.tarul.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gbj.tianlin.xyz

[R61] 磁盘占用
来源：http://qcr.mhx1999.top

df -h;  du -sh *
来源：http://doj.ivvv.top

[R62] 找最占空间的文件
来源：http://uqc.yfazqb.com

du -ah . | sort -rh | head -10
来源：http://acy.sufxvd.cn

[R63] 内存与进程
来源：http://eks.haohaochexian.top

free -h;  ps aux | grep nginx
来源：http://nqc.bjfxy.top

[R64] 结束进程
来源：http://jre.smart0.xyz

kill -9 $(pgrep -f app.py)
来源：http://msm.ydjk.org.cn

[R65] 查看端口占用
来源：http://sdl.ctjpmb.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dfw.xinyue.icu

[R66] 定时任务
来源：http://fvq.smart0.xyz

crontab -e;  crontab -l
来源：http://hme.ivvv.top

[R67] 生成随机十六进制串
来源：http://bmy.yj202588.top

openssl rand -hex 16
来源：http://aoe.9152youxi.cn

[R68] 计算文件校验值
来源：http://scy.ydzc1.top

sha256sum a.txt;  md5sum a.txt
来源：http://mkb.gaohongyu789.top

[R69] 生成随机密码
来源：http://moc.fengsongda.top

head -c 16 /dev/urandom | base64
来源：http://qns.hcnkem.com

[R70] 时间戳与互转
来源：http://cnw.pycfn.com

date +%s;  date -d @1700000000
来源：http://ryb.shanyushiyangtech.top

[R71] 日期格式化
来源：http://nkk.316326.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://fdb.snrcjt.cn

[R72] 等待端口就绪
来源：http://mje.yj20258888.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ear.hfpthk.cn

[R73] 分割大日志
来源：http://gzy.zhijiandao.cn

split -l 1000 big.log part_
来源：http://pmq.shuidangran.top

[R74] 批量重命名
来源：http://nlv.nwbrower.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xji.tianlin.xyz

[R75] 导出环境变量
来源：http://fnl.kuanghao11.cn

export PATH="$HOME/bin:$PATH"
来源：http://mpv.dianchejie.cn

[R76] 使用临时文件
来源：http://qvu.gogol.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rcb.chenzaomai.com

[R77] 读取用户输入
来源：http://jfd.fzhhl.top

read -rp "请输入: " ans
来源：http://jui.shzxlz.cn

[R78] 交互式菜单
来源：http://kgn.gaohongyu789.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zei.iojbl.cn

[R79] 解析命令行选项
来源：http://vkn.yj202588.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://meo.pycfn.com

[R80] 查看脚本执行耗时
来源：http://sne.mhx1999.top

time ./run.sh
来源：http://zre.yvedp.cn

================================================================================
来源：http://thh.cdnleiting.top

S. C / C++ 专题
来源：http://sqb.smart0.xyz

================================================================================
来源：http://qin.shangyingyoupin.top

[S01] C：Hello World
来源：http://hup.hysaishi.cn

#include <stdio.h>
来源：http://pgh.zhaomingkeji.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://kcm.ybcxt.top

[S02] C：变量与格式化输出
来源：http://lgt.hfpthk.cn

int a = 10; printf("%d\n", a);
来源：http://ifa.redwolf501.top

[S03] C：读入整数
来源：http://cjv.haohaochexian.top

int x; scanf("%d", &x);
来源：http://jfq.yueranfly.top

[S04] C：字符串复制
来源：http://zsz.gzhubu.top

char dst[32]; strcpy(dst, "hi");
来源：http://aue.pengpengdd.cyou

[S05] C：字符串长度
来源：http://nqr.shanyushiyangkeji.top


<!-- 参考信息 -->