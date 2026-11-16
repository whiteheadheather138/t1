代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://otc.yanxiufei.cn

[Q22] 排序
来源：http://vpf.snrcjt.cn

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://cpe.haohaochexian.top

[Q23] 分页
来源：http://ofu.sysykeji.top

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://gse.fengsongda.top

[Q24] 去重
来源：http://fsg.jyoumei.cn

SELECT DISTINCT city FROM users;
来源：http://hmv.hnqzz.top

[Q25] 只取前 N 条
来源：http://wle.redwolf501.top

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://ttd.yonumen.top

[Q26] 计数
来源：http://aga.vqdsnc.cn

SELECT COUNT(*) FROM users;
来源：http://vsk.cdnleiting.top

[Q27] 条件计数
来源：http://fyr.xuanzx.com

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://rfv.gogol.net.cn

[Q28] 求和与平均
来源：http://eel.316326.xyz

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://xxh.yangfankeji.com

[Q29] 最大最小值
来源：http://jeh.sysykeji.top

SELECT MAX(age), MIN(age) FROM users;
来源：http://qvn.birdmap.top

[Q30] 分组统计
来源：http://zsf.hesvh.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://acl.ctjpmb.com

[Q31] 分组后过滤
来源：http://myr.cheryme.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://xyh.fanxiaobao.xyz

[Q32] 分组拼接字符串
来源：http://dui.zhengqikj.top

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wzt.hnqzz.top

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://jjy.yvedp.cn

[Q33] 多列分组
来源：http://aer.xinyue.icu

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://gfz.zhoulong.xyz

[Q34] 每组取第一条
来源：http://nrf.jinqigufen.top

SELECT * FROM (
来源：http://bic.tianlin.xyz

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://zxe.ybcxt.top

) t WHERE rn = 1;
来源：http://pdj.zycfv.cn

[Q35] 内连接
来源：http://luk.gotoacloud.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://eqi.ctjpmb.com

[Q36] 左连接
来源：http://zbs.yj202588.top

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://hhp.zhiwuduotai.top

[Q37] 右连接
来源：http://gkz.sweek.top

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://ogh.jianghu66.top

[Q38] 全外连接（PostgreSQL）
来源：http://fmc.c1oappe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://tnj.52xcode.cn

[Q39] 自连接（查上下级）
来源：http://uiq.havefunace.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://nhv.ybcxt.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://ygk.tian-w.cn

[Q40] 交叉连接（笛卡尔积）
来源：http://fkq.316326.xyz

SELECT * FROM colors CROSS JOIN sizes;
来源：http://rsw.aizwys.cn

[Q41] 多表连接
来源：http://yog.chenjidiqi.icu

SELECT o.id, u.name, p.title FROM orders o
来源：http://afs.hammf.cn

JOIN users u ON u.id = o.user_id
来源：http://wnz.feifeiyinyue.top

JOIN products p ON p.id = o.product_id;
来源：http://ipy.quarkkingdee.top

[Q42] 连接条件附加过滤
来源：http://mxy.ydjk.org.cn

SELECT u.name, o.amount FROM users u
来源：http://vgj.zhixingplan.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mrn.guowangkeji.top

[Q43] 标量子查询
来源：http://hmx.shzxlz.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mwh.xingfuxueyuan.xyz

[Q44] IN 子查询
来源：http://awc.quarkkingdee.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://agm.nanxuanxn.top

[Q45] EXISTS 判断存在
来源：http://zfc.cdnleiting.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://src.ybcxt.top

[Q46] NOT EXISTS 判断不存在
来源：http://nss.yongpay.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://icb.daxiang520.top

[Q47] 与平均值比较
来源：http://yev.nanxinkj.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://epk.hywenlv.cn

[Q48] CTE 公用表表达式
来源：http://jib.sjlbkw.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ntl.zhengqikj.top

SELECT * FROM t WHERE c > 5;
来源：http://qcr.ydjk.org.cn

[Q49] 更新单行
来源：http://qce.yongpay.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ewu.ywan-chungtsiang.top

[Q50] 批量更新
来源：http://xyy.jqgfzy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://sgo.yj20258.top

[Q51] 用子查询更新
来源：http://sck.yuanzhike.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://vjv.nanxuanxn.top

[Q52] 删除指定行
来源：http://jzi.fktsv.cn

DELETE FROM users WHERE id = 10;
来源：http://rik.smart0.xyz

[Q53] 按条件删除
来源：http://pct.yuanzhike.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mel.zhaomingkeji.xyz

[Q54] 清空表
来源：http://lch.ctjpmb.com

TRUNCATE TABLE logs;
来源：http://arn.vqdsnc.cn

[Q55] 排名（并列占位）
来源：http://orn.hammf.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fqu.zhijiandao.cn

[Q56] 密集排名（并列不占位）
来源：http://tzx.tarul.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://rqr.sweek.top

[Q57] 行号
来源：http://cgw.zhiwuduotai.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cvy.gaohongyu789.top

[Q58] 累计求和
来源：http://uti.guannengcc.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xxz.cdnleiting.top

[Q59] 分组内累计
来源：http://myn.vqdsnc.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://vmq.snrcjt.cn

[Q60] 取上一行 / 下一行
来源：http://qjr.9152youxi.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://flu.haohaochexian.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gwx.sxryk.cn

[Q61] 移动平均
来源：http://ere.jyoumei.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://vck.cashguo.top

[Q62] 分组占比
来源：http://tla.xuetiantiany.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lgx.vehdjk.com

[Q63] 开启事务
来源：http://exb.hfpthk.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://kvw.yonumen.top

[Q64] 提交事务
来源：http://uqr.gzhubu.top

COMMIT;
来源：http://fvj.hfpthk.cn

[Q65] 回滚事务
来源：http://sht.zdqjudy.top

ROLLBACK;
来源：http://sut.jyoumei.cn

[Q66] 行锁查询
来源：http://bjs.chenjidiqi.icu

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://pio.hnqzz.top

[Q67] 设置隔离级别
来源：http://taa.xuanzx.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vqk.epnwcf.com

[Q68] 保存点
来源：http://jjx.vehdjk.com

SAVEPOINT sp1;
来源：http://vkw.xuetiantiany.cn

ROLLBACK TO sp1;
来源：http://pss.chenzaomai.com

[Q69] 查看执行计划
来源：http://lzl.svipenyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tub.yangfankeji.com

[Q70] 更新统计信息
来源：http://wiy.zycfv.cn

ANALYZE TABLE users;
来源：http://xpn.cashguo.top

[Q71] 查看建表语句
来源：http://jcp.hongshengwenyu.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ngn.redwolf501.top

[Q72] 查看索引
来源：http://kii.hesvh.cn

SHOW INDEX FROM users;
来源：http://yex.nanxuanxn.top

[Q73] 查看表状态
来源：http://lnu.svipenyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tpz.yfazqb.com

[Q74] 强制使用索引
来源：http://tlx.bjfxy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://zsz.jlsjyb.cn

[Q75] 日期格式化
来源：http://oau.shzxlz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://bln.xinyue.icu

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://isl.xuetiantiany.cn

[Q76] 按天统计
来源：http://khq.pycfn.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jlz.zhijiandao.cn

[Q77] 时间加减
来源：http://tvc.ctjpmb.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zby.xziqi.cn

[Q78] 当前时间
来源：http://qtd.fanxiaobao.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rqm.cdnleiting.top

[Q79] 字符串拼接
来源：http://ybr.snrcjt.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ehp.dashuyun.cn

[Q80] 字符串截取
来源：http://hrm.ctjpmb.com

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://otw.dianchejie.cn

[Q81] 字符串替换
来源：http://nki.ppjwa.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rvq.xylfe.cn

[Q82] 字符长度与字节长度
来源：http://kzg.daxiang520.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://qkp.yj202588.top

[Q83] 大小写转换
来源：http://uqz.jlsjyb.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://itc.chenzaomai.com

[Q84] 去除首尾空格
来源：http://vlv.mhx1999.top

SELECT TRIM(name) FROM users;
来源：http://qmt.shanyushiyangkeji.top

[Q85] 数值取整
来源：http://kue.sjlbkw.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jni.wangshuangyany.cn

[Q86] 读取 JSON 字段
来源：http://wgl.jinqigfzy.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mex.fengsongda.top

[Q87] JSON 字段做条件
来源：http://qxh.ybcxt.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ooj.hesvh.cn

[Q88] 行转列（条件聚合）
来源：http://gqk.meibo888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cdp.yonumen.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://xyi.gogol.net.cn

[Q89] 判断表是否存在
来源：http://kpf.jinghuilouyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wys.pengpengdd.cyou

[Q90] 生成序号列
来源：http://whn.gogol.net.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ami.316326.xyz

================================================================================
来源：http://tbj.tianlin.xyz

R. Bash 专题
来源：http://ika.ivvv.top

================================================================================
来源：http://jzu.ydzc1.top

[R01] shebang 与严格模式
来源：http://jxw.nanxinkj.top

#!/usr/bin/env bash
来源：http://byy.tian-w.cn

set -euo pipefail
来源：http://uhd.52xcode.cn

[R02] 变量赋值与使用
来源：http://faj.zhaomingkeji.xyz

name="Tom"; echo "$name"
来源：http://sxt.yfazqb.com

[R03] 只读变量
来源：http://aqp.xingfuxueyuan.xyz

readonly PI=3.14
来源：http://zpk.shanyushiyangkeji.top

[R04] 位置参数
来源：http://jui.cucudq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dei.redwolf501.top

[R05] 参数默认值
来源：http://ycs.xziqi.cn

name="${1:-default}"
来源：http://mmd.iojbl.cn

[R06] 判断命令是否存在
来源：http://qsg.kuanghao11.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vaa.nwbrower.top

[R07] if 判断文件
来源：http://msk.jinghuilouyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ocj.cqqwz.cn

[R08] 数值比较
来源：http://psx.52xcode.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pbn.yanxiufei.cn

[R09] 字符串比较
来源：http://rqb.havefunace.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ire.yfazqb.com

[R10] 正则匹配
来源：http://nqz.cashguo.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ixh.cdnleiting.top

[R11] case 多分支
来源：http://tnc.kuanghao11.cn

case "$1" in
来源：http://oez.fzhhl.top

start) echo "启动" ;;
来源：http://nsq.wangdashe.top

stop)  echo "停止" ;;
来源：http://gem.chenzaomai.com

*)     echo "未知命令" ;;
来源：http://yaw.yueranfly.top

esac
来源：http://aom.hcnkem.com

[R12] for 遍历文件
来源：http://pbf.hnqzz.top

for f in *.txt; do echo "$f"; done
来源：http://fqw.chenjidiqi.icu

[R13] for 计数循环
来源：http://nwh.hnxiangtu.top

for i in {1..10}; do echo "$i"; done
来源：http://gpz.ctjpmb.com

[R14] C 风格 for
来源：http://vno.9152youxi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yph.52xcode.cn

[R15] while 逐行读文件
来源：http://tal.fzhhl.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://jzh.gaohongyu789.top

[R16] until 等待条件
来源：http://kst.dashuyun.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://cft.nanxuanxn.top

[R17] 数组定义与取值
来源：http://yjf.jlsjyb.cn

arr=(a b c); echo "${arr[0]}"
来源：http://xmd.yvedp.cn

[R18] 遍历数组
来源：http://cex.havefunace.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qac.zhoulong.xyz

[R19] 数组长度
来源：http://mri.fktsv.cn

echo "${#arr[@]}"
来源：http://wko.cdnleiting.top

[R20] 关联数组（字典）
来源：http://fsa.chenlongwang.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://suj.uphjek.com

[R21] 字符串长度
来源：http://sdg.ydjk.org.cn

echo "${#s}"
来源：http://zqi.jlsjyb.cn

[R22] 截取子串
来源：http://hhy.tianlin.xyz

echo "${s:0:5}"
来源：http://ldw.guannengcc.top

[R23] 字符串替换
来源：http://kck.chenjidiqi.icu

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ihn.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://ydt.yuanzhike.top

echo "${s^^}"; echo "${s,,}"
来源：http://moa.xinyue.icu

[R25] 去后缀 / 去前缀
来源：http://sdd.yangfankeji.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://qbt.jqgfzy.top

[R26] 命令替换
来源：http://mto.andypj.xyz

now=$(date +%F); echo "$now"
来源：http://fwu.hammf.cn

[R27] 算术展开
来源：http://hpj.yueranfly.top

echo $((1 + 2 * 3))
来源：http://bfj.zhongyouzk.top

[R28] 浮点运算
来源：http://vug.jinyuanbaomall.cn

echo "scale=2; 10/3" | bc
来源：http://hmb.ywan-chungtsiang.top

[R29] 定义函数
来源：http://yfn.fktsv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://aby.wangdashe.top

[R30] 函数返回状态码
来源：http://qki.andypj.xyz

f() { return 0; }; f || echo "失败了"
来源：http://yfw.cheryme.top

[R31] 局部变量
来源：http://bao.sufxvd.cn

f() { local x=1; echo "$x"; }
来源：http://vws.zdqjudy.top

[R32] 参数个数校验
来源：http://hbt.nwbrower.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wys.chenlongwang.top

[R33] 捕获错误并提示行号
来源：http://ipw.shuidangran.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vuh.uphjek.com

[R34] 退出时清理
来源：http://uox.nanxinkj.top

trap 'rm -f "$tmp"' EXIT
来源：http://pmm.hongshengwenyu.top

[R35] 后台执行并等待
来源：http://wvs.fktsv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://tsu.xuanzx.com

[R36] 并发执行多个任务
来源：http://ump.nanxuanxn.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://svh.yangfankeji.com

[R37] 把输出赋给变量
来源：http://glh.yj20258888.top

files=$(ls -1)
来源：http://hjg.daria6918.cn

[R38] 管道串联
来源：http://qbn.pengpengdd.cyou

cat a.txt | grep -i error | wc -l
来源：http://vjh.zdqjudy.top

[R39] 重定向标准输出与错误
来源：http://rtg.hywenlv.cn

cmd > out.log 2>&1
来源：http://mic.ppjwa.cn

[R40] 追加写日志
来源：http://qnz.smart0.xyz

echo "log" >> out.log
来源：http://vrk.ybcxt.top

[R41] 丢弃输出
来源：http://non.guowangkeji.top

cmd >/dev/null 2>&1
来源：http://dak.tanke756.top

[R42] 输入重定向
来源：http://xvc.yongpay.top

wc -l < a.txt
来源：http://zjd.jinghuilouyu.cn

[R43] 按名字查找文件
来源：http://dbf.kuanghao11.cn

find . -name "*.log" -type f
来源：http://gan.vqdsnc.cn

[R44] 按修改时间查找
来源：http://tka.mhx1999.top

find . -mtime -7 -type f
来源：http://dtn.nanxinkj.top

[R45] 批量删除
来源：http://cds.yongpay.top

find . -name "*.tmp" -delete
来源：http://bxx.xuanzx.com

[R46] 递归替换文件内容
来源：http://pgd.shanyushiyangkeji.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://oqr.xuetiantiany.cn

[R47] sed 单行替换
来源：http://uwl.ybcxt.top

sed -i 's/foo/bar/g' a.txt
来源：http://ujw.shanyushiyangtech.top

[R48] awk 取指定列
来源：http://bzm.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://lqi.bjfxy.top

[R49] awk 带条件
来源：http://ghp.jinqigufen.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jov.guannengcc.top

[R50] awk 求和
来源：http://rgy.shzxlz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://lzp.hywenlv.cn

[R51] 排序去重取前几
来源：http://ywr.hnqzz.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gup.shzxlz.cn

[R52] 统计行数
来源：http://pvk.guannengcc.top

wc -l a.txt
来源：http://bsk.sxryk.cn

[R53] 查看文件头与实时尾
来源：http://qaj.zhengqikj.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iac.zhengqikj.top

[R54] 比较两个文件
来源：http://xas.c1oappe.top

diff a.txt b.txt
来源：http://vem.zhijiandao.cn

[R55] 压缩与解压
来源：http://dhv.vehdjk.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wfb.shuidangran.top

[R56] 远程拷贝
来源：http://ndt.yj20258.top

scp file user@host:/path/
来源：http://jzb.yangfankeji.com

[R57] 远程执行命令
来源：http://hpq.hammf.cn

ssh user@host 'uptime'
来源：http://syk.fktsv.cn

[R58] 下载文件
来源：http://jnd.fehbvm.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eaa.shuidangran.top

[R59] 发 POST JSON
来源：http://isn.tarul.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://sru.xuetiantiany.cn

[R60] 只看 HTTP 状态码
来源：http://gvs.xuanzx.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jdo.andypj.xyz

[R61] 磁盘占用
来源：http://jwc.daria6918.cn

df -h;  du -sh *
来源：http://tpf.pycfn.com

[R62] 找最占空间的文件
来源：http://axr.zdbjq.cn

du -ah . | sort -rh | head -10
来源：http://scr.yuxming.cn

[R63] 内存与进程
来源：http://lnx.yueranfly.top

free -h;  ps aux | grep nginx
来源：http://ibn.nanxinkj.top

[R64] 结束进程
来源：http://jrg.cheryme.top

kill -9 $(pgrep -f app.py)
来源：http://sdo.ydzc1.top

[R65] 查看端口占用
来源：http://tuc.chenjidiqi.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qss.feifeiyinyue.top

[R66] 定时任务
来源：http://dxv.guannengcc.top

crontab -e;  crontab -l
来源：http://ghx.iojbl.cn

[R67] 生成随机十六进制串
来源：http://vqp.fzhhl.top

openssl rand -hex 16
来源：http://tju.guannengcc.top

[R68] 计算文件校验值
来源：http://slx.jinqigufen.top

sha256sum a.txt;  md5sum a.txt
来源：http://wyw.jyoumei.cn

[R69] 生成随机密码
来源：http://hrh.9152youxi.cn

head -c 16 /dev/urandom | base64
来源：http://hap.epnwcf.com

[R70] 时间戳与互转
来源：http://act.ivvv.top

date +%s;  date -d @1700000000
来源：http://jkn.jqgufenzy.top

[R71] 日期格式化
来源：http://bse.ppjwa.cn


<!-- 参考信息 -->