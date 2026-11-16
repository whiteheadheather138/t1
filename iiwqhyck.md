代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ofw.0kj1m.cn

[Q26] 计数
来源：http://moc.fehbvm.com

SELECT COUNT(*) FROM users;
来源：http://lif.ivvv.top

[Q27] 条件计数
来源：http://hor.0kj1m.cn

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://efk.gogol.net.cn

[Q28] 求和与平均
来源：http://lcs.yfazqb.com

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://lsk.zdqjudy.top

[Q29] 最大最小值
来源：http://ntp.gogol.net.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://kjf.shangyingyoupin.top

[Q30] 分组统计
来源：http://kkc.chenlongwang.top

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://ifa.pycfn.com

[Q31] 分组后过滤
来源：http://coy.sysykeji.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mpc.jyoumei.cn

[Q32] 分组拼接字符串
来源：http://qcg.ydjk.org.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://nos.jlsjyb.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://hyh.zhongyouzk.top

[Q33] 多列分组
来源：http://crd.fanxiaobao.xyz

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://dfp.tian-w.cn

[Q34] 每组取第一条
来源：http://mnc.hesvh.cn

SELECT * FROM (
来源：http://sbb.bbcook.cn

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xyu.daxiang520.top

) t WHERE rn = 1;
来源：http://llm.daria6918.cn

[Q35] 内连接
来源：http://eoq.yuanzhike.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://dxh.shanyushiyangkeji.top

[Q36] 左连接
来源：http://afy.jianghu66.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hci.chenlongwang.top

[Q37] 右连接
来源：http://lop.aibaodan.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://lsg.dashuyun.cn

[Q38] 全外连接（PostgreSQL）
来源：http://xqk.yuxming.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://ydt.vqdsnc.cn

[Q39] 自连接（查上下级）
来源：http://ntk.hesvh.cn

SELECT e.name, m.name AS manager FROM employees e
来源：http://onq.zdbjq.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://npy.sufxvd.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://tde.zhoulong.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mer.sjlbkw.cn

[Q41] 多表连接
来源：http://med.meibo888.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://viy.shuidangran.top

JOIN users u ON u.id = o.user_id
来源：http://goz.zhongyouzk.top

JOIN products p ON p.id = o.product_id;
来源：http://kxd.jlsjyb.cn

[Q42] 连接条件附加过滤
来源：http://fjm.wangdashe.top

SELECT u.name, o.amount FROM users u
来源：http://guv.snrcjt.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://zav.zhiwuduotai.top

[Q43] 标量子查询
来源：http://jrz.shangyingyoupin.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zix.birdmap.top

[Q44] IN 子查询
来源：http://iku.yfazqb.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://fgm.sweek.top

[Q45] EXISTS 判断存在
来源：http://fdu.daxiang520.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mwg.jinqigufen.top

[Q46] NOT EXISTS 判断不存在
来源：http://vob.shzxlz.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zgd.sufxvd.cn

[Q47] 与平均值比较
来源：http://oei.yuanzhike.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://pdc.jianghu66.top

[Q48] CTE 公用表表达式
来源：http://eof.ppjwa.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://vkx.smart0.xyz

SELECT * FROM t WHERE c > 5;
来源：http://wni.cqqwz.cn

[Q49] 更新单行
来源：http://ujl.0kj1m.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://fqt.shzxlz.cn

[Q50] 批量更新
来源：http://rgd.zhiwuduotai.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://iev.yj202588.top

[Q51] 用子查询更新
来源：http://jhe.xziqi.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://olw.dianchejie.cn

[Q52] 删除指定行
来源：http://agz.pengpengdd.cyou

DELETE FROM users WHERE id = 10;
来源：http://euz.zhiwuduotai.top

[Q53] 按条件删除
来源：http://igi.vehdjk.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ads.sysykeji.top

[Q54] 清空表
来源：http://ajs.daria6918.cn

TRUNCATE TABLE logs;
来源：http://djc.wangshuangyany.cn

[Q55] 排名（并列占位）
来源：http://izd.hongshengwenyu.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dde.nanxuanxn.top

[Q56] 密集排名（并列不占位）
来源：http://zyh.shuidangran.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bkk.yuxming.cn

[Q57] 行号
来源：http://rgj.zhixingplan.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://muo.jqgfzy.top

[Q58] 累计求和
来源：http://lba.xingfuxueyuan.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kor.hfpthk.cn

[Q59] 分组内累计
来源：http://dac.c1oappe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hrp.0kj1m.cn

[Q60] 取上一行 / 下一行
来源：http://sgt.yongpay.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://czj.yuanzhike.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wtc.jiagoushi.top

[Q61] 移动平均
来源：http://fng.yuxming.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cmf.chenjidiqi.icu

[Q62] 分组占比
来源：http://zjm.aibaodan.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yjq.hnxiangtu.top

[Q63] 开启事务
来源：http://oql.sysykeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ibi.zhoulong.xyz

[Q64] 提交事务
来源：http://xpd.haohaochexian.top

COMMIT;
来源：http://wts.jiagoushi.top

[Q65] 回滚事务
来源：http://jbw.yuxming.cn

ROLLBACK;
来源：http://iax.xylfe.cn

[Q66] 行锁查询
来源：http://yyw.sxryk.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pgj.vehdjk.com

[Q67] 设置隔离级别
来源：http://ktr.zhiwuduotai.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zrv.0kj1m.cn

[Q68] 保存点
来源：http://qqh.yonumen.top

SAVEPOINT sp1;
来源：http://yem.tianlin.xyz

ROLLBACK TO sp1;
来源：http://gpt.nanxinkj.top

[Q69] 查看执行计划
来源：http://woi.birdmap.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://cxp.zdqjudy.top

[Q70] 更新统计信息
来源：http://lmc.shanyushiyangtech.top

ANALYZE TABLE users;
来源：http://ilt.jinghuilouyu.cn

[Q71] 查看建表语句
来源：http://vsp.52xcode.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vak.cdnleiting.top

[Q72] 查看索引
来源：http://eij.jlsjyb.cn

SHOW INDEX FROM users;
来源：http://ovp.nanxinkj.top

[Q73] 查看表状态
来源：http://ebq.yuxming.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://qzj.shanyushiyangkeji.top

[Q74] 强制使用索引
来源：http://zwj.quarkkingdee.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nhp.nanxinkj.top

[Q75] 日期格式化
来源：http://wdr.yj20258888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://eri.tian-w.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://vrh.zdqjudy.top

[Q76] 按天统计
来源：http://gqp.fengsongda.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://xyr.ctjpmb.com

[Q77] 时间加减
来源：http://rud.yj20258888.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://cbh.yj202588.top

[Q78] 当前时间
来源：http://wzu.fengsongda.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fss.ydjk.org.cn

[Q79] 字符串拼接
来源：http://ulx.ybcxt.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://dvc.zhiwuduotai.top

[Q80] 字符串截取
来源：http://xyt.birdmap.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xvn.yuxming.cn

[Q81] 字符串替换
来源：http://gxm.cucudq.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vtu.jyoumei.cn

[Q82] 字符长度与字节长度
来源：http://faq.yuanzhike.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wzx.gotoacloud.top

[Q83] 大小写转换
来源：http://sht.xuanzx.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kjl.yangfankeji.com

[Q84] 去除首尾空格
来源：http://czw.jinyuanbaomall.cn

SELECT TRIM(name) FROM users;
来源：http://ckv.fehbvm.com

[Q85] 数值取整
来源：http://cgj.wangdashe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nbb.jinqigfzy.top

[Q86] 读取 JSON 字段
来源：http://bdi.havefunace.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ted.jqgufenzy.top

[Q87] JSON 字段做条件
来源：http://hav.sxryk.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nro.wangshuangyany.cn

[Q88] 行转列（条件聚合）
来源：http://ffz.gzhubu.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aiv.cqqwz.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qkx.zdbjq.cn

[Q89] 判断表是否存在
来源：http://pyf.hesvh.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://noi.aibaodan.cn

[Q90] 生成序号列
来源：http://rsk.tianlin.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pzj.xingfuxueyuan.xyz

================================================================================
来源：http://wes.tianlin.xyz

R. Bash 专题
来源：http://ibg.sufxvd.cn

================================================================================
来源：http://vrq.wangdashe.top

[R01] shebang 与严格模式
来源：http://qmw.meibo888.top

#!/usr/bin/env bash
来源：http://ube.shangyingyoupin.top

set -euo pipefail
来源：http://zug.fanxiaobao.xyz

[R02] 变量赋值与使用
来源：http://zsr.shangyingyoupin.top

name="Tom"; echo "$name"
来源：http://uxn.jinqigfzy.top

[R03] 只读变量
来源：http://ctr.epnwcf.com

readonly PI=3.14
来源：http://mxi.meibo888.top

[R04] 位置参数
来源：http://ewb.jiagoushi.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://eeh.hnqzz.top

[R05] 参数默认值
来源：http://isf.jinqigufen.top

name="${1:-default}"
来源：http://nmf.hywenlv.cn

[R06] 判断命令是否存在
来源：http://exr.mhx1999.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oek.fktsv.cn

[R07] if 判断文件
来源：http://ywp.hnxiangtu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ayo.hnqzz.top

[R08] 数值比较
来源：http://hya.xziqi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://men.yfazqb.com

[R09] 字符串比较
来源：http://qam.tarul.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bmz.0kj1m.cn

[R10] 正则匹配
来源：http://caf.sxryk.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mmy.aibaodan.cn

[R11] case 多分支
来源：http://aog.yj202588.top

case "$1" in
来源：http://tbu.jqgufenzy.top

start) echo "启动" ;;
来源：http://csc.chenzaomai.com

stop)  echo "停止" ;;
来源：http://wdc.fengsongda.top

*)     echo "未知命令" ;;
来源：http://drw.yanxiufei.cn

esac
来源：http://ewo.yuanzhike.top

[R12] for 遍历文件
来源：http://dhx.daxiang520.top

for f in *.txt; do echo "$f"; done
来源：http://kdr.ctjpmb.com

[R13] for 计数循环
来源：http://eas.snrcjt.cn

for i in {1..10}; do echo "$i"; done
来源：http://lwv.52xcode.cn

[R14] C 风格 for
来源：http://mpt.shanyushiyangtech.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wkt.chenzaomai.com

[R15] while 逐行读文件
来源：http://hnd.yongpay.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gsr.zhongyouzk.top

[R16] until 等待条件
来源：http://pqs.c1oappe.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://txq.yonumen.top

[R17] 数组定义与取值
来源：http://ehs.bjfxy.top

arr=(a b c); echo "${arr[0]}"
来源：http://hep.fktsv.cn

[R18] 遍历数组
来源：http://mvn.cashguo.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://llk.fehbvm.com

[R19] 数组长度
来源：http://bog.cucudq.cn

echo "${#arr[@]}"
来源：http://fzj.dashuyun.cn

[R20] 关联数组（字典）
来源：http://xmk.zhixingplan.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hoi.yj20258888.top

[R21] 字符串长度
来源：http://gti.gogol.net.cn

echo "${#s}"
来源：http://psy.pycfn.com

[R22] 截取子串
来源：http://xlm.hongshengwenyu.top

echo "${s:0:5}"
来源：http://aad.shzxlz.cn

[R23] 字符串替换
来源：http://khm.hesvh.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bzj.zhongyouzk.top

[R24] 大小写转换
来源：http://ptl.fzhhl.top

echo "${s^^}"; echo "${s,,}"
来源：http://xkw.vqdsnc.cn

[R25] 去后缀 / 去前缀
来源：http://sru.jinghuilouyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://sle.vehdjk.com

[R26] 命令替换
来源：http://idu.shangyingyoupin.top

now=$(date +%F); echo "$now"
来源：http://xfn.sufxvd.cn

[R27] 算术展开
来源：http://mnq.sufxvd.cn

echo $((1 + 2 * 3))
来源：http://unu.ydjk.org.cn

[R28] 浮点运算
来源：http://ehe.sufxvd.cn

echo "scale=2; 10/3" | bc
来源：http://mqg.cashguo.top

[R29] 定义函数
来源：http://bfm.sjlbkw.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://txz.sweek.top

[R30] 函数返回状态码
来源：http://lon.yangfankeji.com

f() { return 0; }; f || echo "失败了"
来源：http://oah.andypj.xyz

[R31] 局部变量
来源：http://asj.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://mmi.cheryme.top

[R32] 参数个数校验
来源：http://brp.guannengcc.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://rwt.jinyuanbaomall.cn

[R33] 捕获错误并提示行号
来源：http://gah.hysaishi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://sjj.uphjek.com

[R34] 退出时清理
来源：http://kqd.shangyingyoupin.top

trap 'rm -f "$tmp"' EXIT
来源：http://fei.nwbrower.top

[R35] 后台执行并等待
来源：http://rby.pycfn.com

sleep 5 & pid=$!; wait "$pid"
来源：http://pba.nanxinkj.top

[R36] 并发执行多个任务
来源：http://qiz.jianghu66.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mgy.yuanzhike.top

[R37] 把输出赋给变量
来源：http://zda.52xcode.cn

files=$(ls -1)
来源：http://dnw.tianlin.xyz

[R38] 管道串联
来源：http://fuf.nanxuanxn.top

cat a.txt | grep -i error | wc -l
来源：http://gnl.jinghuilouyu.cn

[R39] 重定向标准输出与错误
来源：http://xos.andypj.xyz

cmd > out.log 2>&1
来源：http://vin.xingfuxueyuan.xyz

[R40] 追加写日志
来源：http://zom.jinyuanbaomall.cn

echo "log" >> out.log
来源：http://wzi.yuxming.cn

[R41] 丢弃输出
来源：http://ywi.yonumen.top

cmd >/dev/null 2>&1
来源：http://szp.xylfe.cn

[R42] 输入重定向
来源：http://dqn.shanyushiyangkeji.top

wc -l < a.txt
来源：http://hkl.dashuyun.cn

[R43] 按名字查找文件
来源：http://nal.yonumen.top

find . -name "*.log" -type f
来源：http://wli.zhaomingkeji.xyz

[R44] 按修改时间查找
来源：http://fwo.cashguo.top

find . -mtime -7 -type f
来源：http://waz.nanxuanxn.top

[R45] 批量删除
来源：http://sue.zdqjudy.top

find . -name "*.tmp" -delete
来源：http://qmd.shangyingyoupin.top

[R46] 递归替换文件内容
来源：http://ejm.yvedp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uto.daria6918.cn

[R47] sed 单行替换
来源：http://vco.xuetiantiany.cn

sed -i 's/foo/bar/g' a.txt
来源：http://myn.chenzaomai.com

[R48] awk 取指定列
来源：http://akp.shangyingyoupin.top

awk '{print $1, $3}' a.txt
来源：http://pzn.fzhhl.top

[R49] awk 带条件
来源：http://qmt.havefunace.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wdj.zdbjq.cn

[R50] awk 求和
来源：http://non.fehbvm.com

awk '{s += $2} END {print s}' a.txt
来源：http://xdp.yueranfly.top

[R51] 排序去重取前几
来源：http://vju.zhixingplan.top

sort a.txt | uniq -c | sort -rn | head
来源：http://yag.meibo888.top

[R52] 统计行数
来源：http://omf.haohaochexian.top

wc -l a.txt
来源：http://xju.gotoacloud.top

[R53] 查看文件头与实时尾
来源：http://aap.zdbjq.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gss.fktsv.cn

[R54] 比较两个文件
来源：http://frk.kuanghao11.cn

diff a.txt b.txt
来源：http://kde.kuanghao11.cn

[R55] 压缩与解压
来源：http://ctn.uphjek.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dyn.sufxvd.cn

[R56] 远程拷贝
来源：http://vkb.fengsongda.top

scp file user@host:/path/
来源：http://glc.316326.xyz

[R57] 远程执行命令
来源：http://xnf.meibo888.top

ssh user@host 'uptime'
来源：http://qib.tian-w.cn

[R58] 下载文件
来源：http://vbp.havefunace.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://icb.sxryk.cn

[R59] 发 POST JSON
来源：http://enq.fengsongda.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://eju.cheryme.top

[R60] 只看 HTTP 状态码
来源：http://ael.bjfxy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://emm.jinqigufen.top

[R61] 磁盘占用
来源：http://fgm.sufxvd.cn

df -h;  du -sh *
来源：http://isf.zdbjq.cn

[R62] 找最占空间的文件
来源：http://lsl.quarkkingdee.top

du -ah . | sort -rh | head -10
来源：http://bbj.yvedp.cn

[R63] 内存与进程
来源：http://cpf.gaohongyu789.top

free -h;  ps aux | grep nginx
来源：http://ckd.yueranfly.top

[R64] 结束进程
来源：http://afs.chenlongwang.top

kill -9 $(pgrep -f app.py)
来源：http://rsz.sysykeji.top

[R65] 查看端口占用
来源：http://tsv.cheryme.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://beq.tanke756.top

[R66] 定时任务
来源：http://yib.hfpthk.cn

crontab -e;  crontab -l
来源：http://jzx.fzhhl.top

[R67] 生成随机十六进制串
来源：http://fds.ppjwa.cn

openssl rand -hex 16
来源：http://gvv.kuanghao11.cn

[R68] 计算文件校验值
来源：http://vbo.ywan-chungtsiang.top

sha256sum a.txt;  md5sum a.txt
来源：http://lsi.shuidangran.top

[R69] 生成随机密码
来源：http://hem.zhoulong.xyz

head -c 16 /dev/urandom | base64
来源：http://klu.pengpengdd.cyou

[R70] 时间戳与互转
来源：http://jjk.shangyingyoupin.top

date +%s;  date -d @1700000000
来源：http://fhg.hnxiangtu.top

[R71] 日期格式化
来源：http://tmv.smart0.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://ptc.hnxiangtu.top

[R72] 等待端口就绪
来源：http://byh.ybcxt.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jrz.haohaochexian.top

[R73] 分割大日志
来源：http://udc.jinqigufen.top

split -l 1000 big.log part_
来源：http://rwa.zycfv.cn

[R74] 批量重命名
来源：http://xvu.jinqigufen.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://drt.yvedp.cn

[R75] 导出环境变量
来源：http://qef.xziqi.cn


<!-- 参考信息 -->