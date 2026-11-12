代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://opr.yuanzhike.top

[Q30] 分组统计
来源：http://cvj.yongpay.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://por.zhiwuduotai.top

[Q31] 分组后过滤
来源：http://egg.cashguo.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://dif.cheryme.top

[Q32] 分组拼接字符串
来源：http://mhy.jinqigfzy.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://opr.gzhubu.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://bcu.mhx1999.top

[Q33] 多列分组
来源：http://ywp.fanxiaobao.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dcg.smart0.xyz

[Q34] 每组取第一条
来源：http://aij.yj202588.top

SELECT * FROM (
来源：http://dzq.xinyue.icu

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://uef.snrcjt.cn

) t WHERE rn = 1;
来源：http://ehc.fzhhl.top

[Q35] 内连接
来源：http://oel.jinqigfzy.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://whp.c1oappe.top

[Q36] 左连接
来源：http://ndz.guannengcc.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://kiz.feifeiyinyue.top

[Q37] 右连接
来源：http://auq.hammf.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://fch.jqgfzy.top

[Q38] 全外连接（PostgreSQL）
来源：http://pcb.ywan-chungtsiang.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://dlr.bjfxy.top

[Q39] 自连接（查上下级）
来源：http://lyb.yueranfly.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://qol.ybcxt.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://dns.zdbjq.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://dde.xingfuxueyuan.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://fsh.jianghu66.top

[Q41] 多表连接
来源：http://eme.ywan-chungtsiang.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bqa.guannengcc.top

JOIN users u ON u.id = o.user_id
来源：http://lhh.sxryk.cn

JOIN products p ON p.id = o.product_id;
来源：http://hau.ybcxt.top

[Q42] 连接条件附加过滤
来源：http://piv.jqgufenzy.top

SELECT u.name, o.amount FROM users u
来源：http://mto.52xcode.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://pid.guowangkeji.top

[Q43] 标量子查询
来源：http://ncj.jianghu66.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://jxn.hcnkem.com

[Q44] IN 子查询
来源：http://jqm.hesvh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://uge.hfpthk.cn

[Q45] EXISTS 判断存在
来源：http://qvy.chenjidiqi.icu

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://etd.jiagoushi.top

[Q46] NOT EXISTS 判断不存在
来源：http://fxh.zhengqikj.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://eft.hnqzz.top

[Q47] 与平均值比较
来源：http://gos.shanyushiyangtech.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mup.xuanzx.com

[Q48] CTE 公用表表达式
来源：http://jiq.9152youxi.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dew.vehdjk.com

SELECT * FROM t WHERE c > 5;
来源：http://tgt.smart0.xyz

[Q49] 更新单行
来源：http://fqd.cashguo.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://grm.ehwqpu.com

[Q50] 批量更新
来源：http://nxn.c1oappe.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://kwy.daxiang520.top

[Q51] 用子查询更新
来源：http://urb.cqqwz.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://afi.jinghuilouyu.cn

[Q52] 删除指定行
来源：http://sqv.tianlin.xyz

DELETE FROM users WHERE id = 10;
来源：http://ahr.daria6918.cn

[Q53] 按条件删除
来源：http://jnt.xuetiantiany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cot.yj20258888.top

[Q54] 清空表
来源：http://xdf.xylfe.cn

TRUNCATE TABLE logs;
来源：http://lkh.bjfxy.top

[Q55] 排名（并列占位）
来源：http://avs.yuxming.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yzr.ywan-chungtsiang.top

[Q56] 密集排名（并列不占位）
来源：http://oer.zhengqikj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wzp.uphjek.com

[Q57] 行号
来源：http://agc.fzhhl.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lpg.hnqzz.top

[Q58] 累计求和
来源：http://svf.jinqigufen.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rrs.52xcode.cn

[Q59] 分组内累计
来源：http://sut.zhongyouzk.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://rvh.tanke756.top

[Q60] 取上一行 / 下一行
来源：http://xdn.svipenyu.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tps.jlsjyb.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dec.mhx1999.top

[Q61] 移动平均
来源：http://zql.shangyingyoupin.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://otg.316326.xyz

[Q62] 分组占比
来源：http://epl.snrcjt.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gia.smart0.xyz

[Q63] 开启事务
来源：http://sfo.meibo888.top

START TRANSACTION;                -- 或 BEGIN
来源：http://tds.ppjwa.cn

[Q64] 提交事务
来源：http://gba.yueranfly.top

COMMIT;
来源：http://vmh.kuanghao11.cn

[Q65] 回滚事务
来源：http://msg.guannengcc.top

ROLLBACK;
来源：http://uvl.zhoulong.xyz

[Q66] 行锁查询
来源：http://dwd.snrcjt.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jgs.ivvv.top

[Q67] 设置隔离级别
来源：http://xyi.jqgufenzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://drd.zhiwuduotai.top

[Q68] 保存点
来源：http://leh.hammf.cn

SAVEPOINT sp1;
来源：http://kzd.aizwys.cn

ROLLBACK TO sp1;
来源：http://nqh.fanxiaobao.xyz

[Q69] 查看执行计划
来源：http://onw.haohaochexian.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fwz.yueranfly.top

[Q70] 更新统计信息
来源：http://fyh.ctjpmb.com

ANALYZE TABLE users;
来源：http://rex.fengsongda.top

[Q71] 查看建表语句
来源：http://awd.hnxiangtu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://apc.vqdsnc.cn

[Q72] 查看索引
来源：http://hyn.jqgfzy.top

SHOW INDEX FROM users;
来源：http://hqn.zhoulong.xyz

[Q73] 查看表状态
来源：http://wei.sweek.top

SHOW TABLE STATUS LIKE 'users';
来源：http://yfc.jlsjyb.cn

[Q74] 强制使用索引
来源：http://isj.gaohongyu789.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ymx.hfpthk.cn

[Q75] 日期格式化
来源：http://rkt.yonumen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gxu.feifeiyinyue.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ryo.316326.xyz

[Q76] 按天统计
来源：http://glf.hfpthk.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yzc.vqdsnc.cn

[Q77] 时间加减
来源：http://mfk.kuanghao11.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gyh.guowangkeji.top

[Q78] 当前时间
来源：http://ero.hongshengwenyu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nda.tanke756.top

[Q79] 字符串拼接
来源：http://pvc.chenzaomai.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://lfz.cucudq.cn

[Q80] 字符串截取
来源：http://sqs.yj20258888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://tng.daria6918.cn

[Q81] 字符串替换
来源：http://ihv.yanxiufei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://xgu.fengsongda.top

[Q82] 字符长度与字节长度
来源：http://imw.ydzc1.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kha.ehwqpu.com

[Q83] 大小写转换
来源：http://pdt.hammf.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pim.sxryk.cn

[Q84] 去除首尾空格
来源：http://tea.birdmap.top

SELECT TRIM(name) FROM users;
来源：http://opz.shangyingyoupin.top

[Q85] 数值取整
来源：http://vry.shanyushiyangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rzs.jqgufenzy.top

[Q86] 读取 JSON 字段
来源：http://chb.yueranfly.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://iaf.daria6918.cn

[Q87] JSON 字段做条件
来源：http://fhm.jinghuilouyu.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://log.tanke756.top

[Q88] 行转列（条件聚合）
来源：http://zac.aizwys.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fcx.epnwcf.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dfb.zycfv.cn

[Q89] 判断表是否存在
来源：http://nkt.jlsjyb.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xkw.cqqwz.cn

[Q90] 生成序号列
来源：http://beb.fanxiaobao.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sdu.yuanzhike.top

================================================================================
来源：http://ckd.ehwqpu.com

R. Bash 专题
来源：http://dma.ppjwa.cn

================================================================================
来源：http://vug.cucudq.cn

[R01] shebang 与严格模式
来源：http://xer.uphjek.com

#!/usr/bin/env bash
来源：http://ibl.jinghuilouyu.cn

set -euo pipefail
来源：http://fxk.xingfuxueyuan.xyz

[R02] 变量赋值与使用
来源：http://pir.yvedp.cn

name="Tom"; echo "$name"
来源：http://ilj.hammf.cn

[R03] 只读变量
来源：http://mrn.zdbjq.cn

readonly PI=3.14
来源：http://npa.hnxiangtu.top

[R04] 位置参数
来源：http://bof.meibo888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://smx.jiagoushi.top

[R05] 参数默认值
来源：http://ylg.0kj1m.cn

name="${1:-default}"
来源：http://twh.bbcook.cn

[R06] 判断命令是否存在
来源：http://nek.yangfankeji.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mwi.chenzaomai.com

[R07] if 判断文件
来源：http://eso.yj20258.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ukm.andypj.xyz

[R08] 数值比较
来源：http://tss.xziqi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://wbg.smart0.xyz

[R09] 字符串比较
来源：http://lai.xziqi.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://vti.cdnleiting.top

[R10] 正则匹配
来源：http://nqe.birdmap.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pxb.nwbrower.top

[R11] case 多分支
来源：http://dbd.ivvv.top

case "$1" in
来源：http://vyw.aibaodan.cn

start) echo "启动" ;;
来源：http://dwg.shanyushiyangtech.top

stop)  echo "停止" ;;
来源：http://hrq.zhongyouzk.top

*)     echo "未知命令" ;;
来源：http://ftk.gotoacloud.top

esac
来源：http://zqv.quarkkingdee.top

[R12] for 遍历文件
来源：http://hvr.yvedp.cn

for f in *.txt; do echo "$f"; done
来源：http://cgd.dashuyun.cn

[R13] for 计数循环
来源：http://ulq.redwolf501.top

for i in {1..10}; do echo "$i"; done
来源：http://max.xuetiantiany.cn

[R14] C 风格 for
来源：http://erd.sweek.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nhx.shangyingyoupin.top

[R15] while 逐行读文件
来源：http://cqy.wangdashe.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fby.yongpay.top

[R16] until 等待条件
来源：http://mcv.vehdjk.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iiv.pycfn.com

[R17] 数组定义与取值
来源：http://hbk.jyoumei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://upt.guannengcc.top

[R18] 遍历数组
来源：http://gwx.hongshengwenyu.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tga.fanxiaobao.xyz

[R19] 数组长度
来源：http://nnr.sweek.top

echo "${#arr[@]}"
来源：http://geg.yongpay.top

[R20] 关联数组（字典）
来源：http://hxr.yj202588.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kdq.havefunace.top

[R21] 字符串长度
来源：http://dqf.316326.xyz

echo "${#s}"
来源：http://tep.chenzaomai.com

[R22] 截取子串
来源：http://gqm.ivvv.top

echo "${s:0:5}"
来源：http://ybl.xingfuxueyuan.xyz

[R23] 字符串替换
来源：http://jau.yvedp.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://quj.316326.xyz

[R24] 大小写转换
来源：http://uql.dianchejie.cn

echo "${s^^}"; echo "${s,,}"
来源：http://iqw.ybcxt.top

[R25] 去后缀 / 去前缀
来源：http://hak.316326.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://nxw.ivvv.top

[R26] 命令替换
来源：http://cwc.andypj.xyz

now=$(date +%F); echo "$now"
来源：http://xvd.haohaochexian.top

[R27] 算术展开
来源：http://osb.jinyuanbaomall.cn

echo $((1 + 2 * 3))
来源：http://cmg.tianlin.xyz

[R28] 浮点运算
来源：http://kld.xinyue.icu

echo "scale=2; 10/3" | bc
来源：http://meg.cqqwz.cn

[R29] 定义函数
来源：http://iij.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://kdg.52xcode.cn

[R30] 函数返回状态码
来源：http://qnn.jinqigfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://dcx.hysaishi.cn

[R31] 局部变量
来源：http://piv.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://iop.shuidangran.top

[R32] 参数个数校验
来源：http://ede.yangfankeji.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wnr.bjfxy.top

[R33] 捕获错误并提示行号
来源：http://izw.tianlin.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pgt.shanyushiyangtech.top

[R34] 退出时清理
来源：http://meb.hnqzz.top

trap 'rm -f "$tmp"' EXIT
来源：http://cwj.epnwcf.com

[R35] 后台执行并等待
来源：http://dov.fzhhl.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vgb.nanxuanxn.top

[R36] 并发执行多个任务
来源：http://hju.yueranfly.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://qpq.316326.xyz

[R37] 把输出赋给变量
来源：http://pad.hnxiangtu.top

files=$(ls -1)
来源：http://qvq.nwbrower.top

[R38] 管道串联
来源：http://xcm.sjlbkw.cn

cat a.txt | grep -i error | wc -l
来源：http://nes.yj20258888.top

[R39] 重定向标准输出与错误
来源：http://rvq.aizwys.cn

cmd > out.log 2>&1
来源：http://ord.jlsjyb.cn

[R40] 追加写日志
来源：http://vaf.0kj1m.cn

echo "log" >> out.log
来源：http://vey.gogol.net.cn

[R41] 丢弃输出
来源：http://olg.yanxiufei.cn

cmd >/dev/null 2>&1
来源：http://pno.yuanzhike.top

[R42] 输入重定向
来源：http://mgs.guannengcc.top

wc -l < a.txt
来源：http://irb.sufxvd.cn

[R43] 按名字查找文件
来源：http://sfz.xinyue.icu

find . -name "*.log" -type f
来源：http://uef.yfazqb.com

[R44] 按修改时间查找
来源：http://aqy.fktsv.cn

find . -mtime -7 -type f
来源：http://nce.yueranfly.top

[R45] 批量删除
来源：http://cwl.pycfn.com

find . -name "*.tmp" -delete
来源：http://lor.epnwcf.com

[R46] 递归替换文件内容
来源：http://uxn.zdbjq.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qei.zdbjq.cn

[R47] sed 单行替换
来源：http://hmi.sweek.top

sed -i 's/foo/bar/g' a.txt
来源：http://jvx.jqgufenzy.top

[R48] awk 取指定列
来源：http://jyk.xinyue.icu

awk '{print $1, $3}' a.txt
来源：http://xwj.meibo888.top

[R49] awk 带条件
来源：http://kgw.dianchejie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gke.zycfv.cn

[R50] awk 求和
来源：http://yey.shangyingyoupin.top

awk '{s += $2} END {print s}' a.txt
来源：http://cub.cqqwz.cn

[R51] 排序去重取前几
来源：http://uhg.hnxiangtu.top

sort a.txt | uniq -c | sort -rn | head
来源：http://oqu.andypj.xyz

[R52] 统计行数
来源：http://jdx.sufxvd.cn

wc -l a.txt
来源：http://idk.sxryk.cn

[R53] 查看文件头与实时尾
来源：http://uhd.hesvh.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://swn.hammf.cn

[R54] 比较两个文件
来源：http://kgz.zdqjudy.top

diff a.txt b.txt
来源：http://gci.daxiang520.top

[R55] 压缩与解压
来源：http://ctz.bjfxy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jcz.cheryme.top

[R56] 远程拷贝
来源：http://ibw.chenjidiqi.icu

scp file user@host:/path/
来源：http://imk.yanxiufei.cn

[R57] 远程执行命令
来源：http://rpj.xuanzx.com

ssh user@host 'uptime'
来源：http://fwn.yj20258.top

[R58] 下载文件
来源：http://mnj.iojbl.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pkp.jinghuilouyu.cn

[R59] 发 POST JSON
来源：http://dhl.yj20258.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ifa.svipenyu.cn

[R60] 只看 HTTP 状态码
来源：http://kuc.birdmap.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tio.ywan-chungtsiang.top

[R61] 磁盘占用
来源：http://umy.cucudq.cn

df -h;  du -sh *
来源：http://mkc.birdmap.top

[R62] 找最占空间的文件
来源：http://zpa.zycfv.cn

du -ah . | sort -rh | head -10
来源：http://bsq.ydjk.org.cn

[R63] 内存与进程
来源：http://jan.ydjk.org.cn

free -h;  ps aux | grep nginx
来源：http://tlk.fanxiaobao.xyz

[R64] 结束进程
来源：http://lpv.hywenlv.cn

kill -9 $(pgrep -f app.py)
来源：http://uin.aibaodan.cn

[R65] 查看端口占用
来源：http://tbp.epnwcf.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hmk.quarkkingdee.top

[R66] 定时任务
来源：http://nhq.tarul.cn

crontab -e;  crontab -l
来源：http://cny.mhx1999.top

[R67] 生成随机十六进制串
来源：http://avi.ehwqpu.com

openssl rand -hex 16
来源：http://yrh.jyoumei.cn

[R68] 计算文件校验值
来源：http://wvi.dianchejie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ndw.yangfankeji.com

[R69] 生成随机密码
来源：http://zat.fanxiaobao.xyz

head -c 16 /dev/urandom | base64
来源：http://mfc.zdqjudy.top

[R70] 时间戳与互转
来源：http://dpu.nwbrower.top

date +%s;  date -d @1700000000
来源：http://dgk.nwbrower.top

[R71] 日期格式化
来源：http://qcy.andypj.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://lko.ydzc1.top

[R72] 等待端口就绪
来源：http://jtf.hcnkem.com

until nc -z localhost 3306; do sleep 1; done
来源：http://nyq.xuanzx.com

[R73] 分割大日志
来源：http://mky.dashuyun.cn

split -l 1000 big.log part_
来源：http://wtq.cqqwz.cn

[R74] 批量重命名
来源：http://iiw.tanke756.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://syc.cucudq.cn

[R75] 导出环境变量
来源：http://xzv.guowangkeji.top

export PATH="$HOME/bin:$PATH"
来源：http://hhf.yj202588.top

[R76] 使用临时文件
来源：http://oiz.hcnkem.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ago.jqgfzy.top

[R77] 读取用户输入
来源：http://otv.hesvh.cn

read -rp "请输入: " ans
来源：http://bdw.yueranfly.top

[R78] 交互式菜单
来源：http://mzm.fzhhl.top

select opt in a b c; do echo "$opt"; break; done
来源：http://fvg.jinqigufen.top

[R79] 解析命令行选项
来源：http://wsm.tarul.cn


<!-- 参考信息 -->