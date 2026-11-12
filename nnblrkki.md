代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://uia.yuxming.cn

[Q28] 求和与平均
来源：http://zly.wangshuangyany.cn

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wkj.yj202588.top

[Q29] 最大最小值
来源：http://lhy.ydjk.org.cn

SELECT MAX(age), MIN(age) FROM users;
来源：http://jzn.yueranfly.top

[Q30] 分组统计
来源：http://kwd.yvedp.cn

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://vio.andypj.xyz

[Q31] 分组后过滤
来源：http://cax.zdqjudy.top

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://frn.yj20258.top

[Q32] 分组拼接字符串
来源：http://eav.hywenlv.cn

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://jft.yuxming.cn

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://vaw.hcnkem.com

[Q33] 多列分组
来源：http://den.c1oappe.top

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://azv.daria6918.cn

[Q34] 每组取第一条
来源：http://bnu.fehbvm.com

SELECT * FROM (
来源：http://cev.ehwqpu.com

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://xzq.shuidangran.top

) t WHERE rn = 1;
来源：http://wlj.jlsjyb.cn

[Q35] 内连接
来源：http://nbj.jinqigufen.top

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://lrt.ppjwa.cn

[Q36] 左连接
来源：http://wnk.sufxvd.cn

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://uac.fanxiaobao.xyz

[Q37] 右连接
来源：http://gtx.yvedp.cn

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://cif.kuanghao11.cn

[Q38] 全外连接（PostgreSQL）
来源：http://kfq.yanxiufei.cn

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://bqx.dashuyun.cn

[Q39] 自连接（查上下级）
来源：http://uex.haohaochexian.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://utv.yfazqb.com

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://qwm.gzhubu.top

[Q40] 交叉连接（笛卡尔积）
来源：http://cdj.nanxinkj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://xys.tanke756.top

[Q41] 多表连接
来源：http://mnx.zycfv.cn

SELECT o.id, u.name, p.title FROM orders o
来源：http://vpy.fengsongda.top

JOIN users u ON u.id = o.user_id
来源：http://vwi.shangyingyoupin.top

JOIN products p ON p.id = o.product_id;
来源：http://enh.zhiwuduotai.top

[Q42] 连接条件附加过滤
来源：http://vao.quarkkingdee.top

SELECT u.name, o.amount FROM users u
来源：http://ukb.zdbjq.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://yep.cheryme.top

[Q43] 标量子查询
来源：http://czu.yj202588.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://suc.zhengqikj.top

[Q44] IN 子查询
来源：http://zxh.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mlm.daxiang520.top

[Q45] EXISTS 判断存在
来源：http://pkm.andypj.xyz

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zpl.xingfuxueyuan.xyz

[Q46] NOT EXISTS 判断不存在
来源：http://wif.9152youxi.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wjr.tarul.cn

[Q47] 与平均值比较
来源：http://nnh.shzxlz.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://tmc.jinqigfzy.top

[Q48] CTE 公用表表达式
来源：http://fqg.xylfe.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://tfr.zhoulong.xyz

SELECT * FROM t WHERE c > 5;
来源：http://uqo.andypj.xyz

[Q49] 更新单行
来源：http://fvo.ppjwa.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://dud.zhixingplan.top

[Q50] 批量更新
来源：http://orw.daxiang520.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://inp.shangyingyoupin.top

[Q51] 用子查询更新
来源：http://ovn.ctjpmb.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mcs.zhongyouzk.top

[Q52] 删除指定行
来源：http://skh.xziqi.cn

DELETE FROM users WHERE id = 10;
来源：http://jrn.feifeiyinyue.top

[Q53] 按条件删除
来源：http://aak.nanxuanxn.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gua.bjfxy.top

[Q54] 清空表
来源：http://nvt.redwolf501.top

TRUNCATE TABLE logs;
来源：http://und.yuanzhike.top

[Q55] 排名（并列占位）
来源：http://cra.cashguo.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://nyi.yj20258.top

[Q56] 密集排名（并列不占位）
来源：http://pwa.sxryk.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mhq.yanxiufei.cn

[Q57] 行号
来源：http://ltz.vehdjk.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ajf.snrcjt.cn

[Q58] 累计求和
来源：http://qpe.ehwqpu.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mfo.zhoulong.xyz

[Q59] 分组内累计
来源：http://txk.sufxvd.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lmo.guowangkeji.top

[Q60] 取上一行 / 下一行
来源：http://yew.hnxiangtu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dvc.ybcxt.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ugu.jiagoushi.top

[Q61] 移动平均
来源：http://plb.ehwqpu.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gdd.sysykeji.top

[Q62] 分组占比
来源：http://acw.meibo888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kcj.birdmap.top

[Q63] 开启事务
来源：http://hez.smart0.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://hin.316326.xyz

[Q64] 提交事务
来源：http://guk.kuanghao11.cn

COMMIT;
来源：http://pfu.yj20258888.top

[Q65] 回滚事务
来源：http://iod.pengpengdd.cyou

ROLLBACK;
来源：http://ksz.jlsjyb.cn

[Q66] 行锁查询
来源：http://dck.tanke756.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eul.svipenyu.cn

[Q67] 设置隔离级别
来源：http://zop.jqgfzy.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rvf.fengsongda.top

[Q68] 保存点
来源：http://cum.yangfankeji.com

SAVEPOINT sp1;
来源：http://biu.zhongyouzk.top

ROLLBACK TO sp1;
来源：http://vrl.cucudq.cn

[Q69] 查看执行计划
来源：http://qjh.ybcxt.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mhb.cdnleiting.top

[Q70] 更新统计信息
来源：http://lqp.svipenyu.cn

ANALYZE TABLE users;
来源：http://veu.hnqzz.top

[Q71] 查看建表语句
来源：http://luz.yanxiufei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://akv.hesvh.cn

[Q72] 查看索引
来源：http://wcr.dianchejie.cn

SHOW INDEX FROM users;
来源：http://rwy.cqqwz.cn

[Q73] 查看表状态
来源：http://bxi.zhiwuduotai.top

SHOW TABLE STATUS LIKE 'users';
来源：http://vqm.wangdashe.top

[Q74] 强制使用索引
来源：http://fan.shanyushiyangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wyc.fanxiaobao.xyz

[Q75] 日期格式化
来源：http://rwy.ctjpmb.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://pis.xingfuxueyuan.xyz

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://jar.ywan-chungtsiang.top

[Q76] 按天统计
来源：http://jyq.svipenyu.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://gdj.andypj.xyz

[Q77] 时间加减
来源：http://sbz.vqdsnc.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nuc.hammf.cn

[Q78] 当前时间
来源：http://xvx.cashguo.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hbb.epnwcf.com

[Q79] 字符串拼接
来源：http://wbr.tanke756.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uuk.pengpengdd.cyou

[Q80] 字符串截取
来源：http://usi.nanxinkj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://dqv.ydzc1.top

[Q81] 字符串替换
来源：http://erx.chenzaomai.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jjc.kuanghao11.cn

[Q82] 字符长度与字节长度
来源：http://khz.hongshengwenyu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wmp.ehwqpu.com

[Q83] 大小写转换
来源：http://arf.tanke756.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://bsc.gaohongyu789.top

[Q84] 去除首尾空格
来源：http://vck.cucudq.cn

SELECT TRIM(name) FROM users;
来源：http://zgc.birdmap.top

[Q85] 数值取整
来源：http://tfq.yangfankeji.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ocy.vqdsnc.cn

[Q86] 读取 JSON 字段
来源：http://lyw.zhengqikj.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rjq.dianchejie.cn

[Q87] JSON 字段做条件
来源：http://uxe.aibaodan.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ydq.fktsv.cn

[Q88] 行转列（条件聚合）
来源：http://peh.ivvv.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dra.yvedp.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kqq.ppjwa.cn

[Q89] 判断表是否存在
来源：http://pfi.yanxiufei.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://dhr.gzhubu.top

[Q90] 生成序号列
来源：http://two.jiagoushi.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jfq.gaohongyu789.top

================================================================================
来源：http://yvx.fehbvm.com

R. Bash 专题
来源：http://vdo.tian-w.cn

================================================================================
来源：http://ruy.gotoacloud.top

[R01] shebang 与严格模式
来源：http://exh.zycfv.cn

#!/usr/bin/env bash
来源：http://qww.jyoumei.cn

set -euo pipefail
来源：http://wjg.jiagoushi.top

[R02] 变量赋值与使用
来源：http://hnz.tianlin.xyz

name="Tom"; echo "$name"
来源：http://txo.yj20258888.top

[R03] 只读变量
来源：http://dek.yanxiufei.cn

readonly PI=3.14
来源：http://xsy.feifeiyinyue.top

[R04] 位置参数
来源：http://rxs.ivvv.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vhs.ivvv.top

[R05] 参数默认值
来源：http://dlv.hfpthk.cn

name="${1:-default}"
来源：http://lru.tarul.cn

[R06] 判断命令是否存在
来源：http://gaq.hnxiangtu.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rfc.daxiang520.top

[R07] if 判断文件
来源：http://qme.hesvh.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aco.iojbl.cn

[R08] 数值比较
来源：http://mvv.daria6918.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://pmw.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://qeg.zhoulong.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://yly.c1oappe.top

[R10] 正则匹配
来源：http://jsr.yuxming.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pvt.uphjek.com

[R11] case 多分支
来源：http://msd.meibo888.top

case "$1" in
来源：http://jrv.fzhhl.top

start) echo "启动" ;;
来源：http://kdi.aizwys.cn

stop)  echo "停止" ;;
来源：http://gte.haohaochexian.top

*)     echo "未知命令" ;;
来源：http://gyi.chenjidiqi.icu

esac
来源：http://onk.hesvh.cn

[R12] for 遍历文件
来源：http://kgh.guannengcc.top

for f in *.txt; do echo "$f"; done
来源：http://zkp.shzxlz.cn

[R13] for 计数循环
来源：http://bsz.kuanghao11.cn

for i in {1..10}; do echo "$i"; done
来源：http://wih.andypj.xyz

[R14] C 风格 for
来源：http://qev.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zxs.daxiang520.top

[R15] while 逐行读文件
来源：http://urr.kuanghao11.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://dzy.jiagoushi.top

[R16] until 等待条件
来源：http://kcs.sysykeji.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://nve.nwbrower.top

[R17] 数组定义与取值
来源：http://fzi.c1oappe.top

arr=(a b c); echo "${arr[0]}"
来源：http://iag.xinyue.icu

[R18] 遍历数组
来源：http://ual.xingfuxueyuan.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://lqu.chenlongwang.top

[R19] 数组长度
来源：http://ysm.gogol.net.cn

echo "${#arr[@]}"
来源：http://kih.ywan-chungtsiang.top

[R20] 关联数组（字典）
来源：http://dhd.sxryk.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mes.uphjek.com

[R21] 字符串长度
来源：http://ywx.zhongyouzk.top

echo "${#s}"
来源：http://afs.xuetiantiany.cn

[R22] 截取子串
来源：http://gdi.zhiwuduotai.top

echo "${s:0:5}"
来源：http://lqw.ppjwa.cn

[R23] 字符串替换
来源：http://skv.vqdsnc.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://czb.shangyingyoupin.top

[R24] 大小写转换
来源：http://qrz.bbcook.cn

echo "${s^^}"; echo "${s,,}"
来源：http://hau.gogol.net.cn

[R25] 去后缀 / 去前缀
来源：http://otb.kuanghao11.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://vrl.sysykeji.top

[R26] 命令替换
来源：http://vwx.yj20258.top

now=$(date +%F); echo "$now"
来源：http://znz.xziqi.cn

[R27] 算术展开
来源：http://yws.pycfn.com

echo $((1 + 2 * 3))
来源：http://toj.shangyingyoupin.top

[R28] 浮点运算
来源：http://xzm.redwolf501.top

echo "scale=2; 10/3" | bc
来源：http://iqf.jinqigfzy.top

[R29] 定义函数
来源：http://hoa.feifeiyinyue.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hcy.chenjidiqi.icu

[R30] 函数返回状态码
来源：http://hgh.gzhubu.top

f() { return 0; }; f || echo "失败了"
来源：http://aty.quarkkingdee.top

[R31] 局部变量
来源：http://tki.zhijiandao.cn

f() { local x=1; echo "$x"; }
来源：http://yjv.jlsjyb.cn

[R32] 参数个数校验
来源：http://mmb.zhaomingkeji.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://akr.zdqjudy.top

[R33] 捕获错误并提示行号
来源：http://dor.wangdashe.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://smf.shanyushiyangkeji.top

[R34] 退出时清理
来源：http://gte.tarul.cn

trap 'rm -f "$tmp"' EXIT
来源：http://soa.hammf.cn

[R35] 后台执行并等待
来源：http://zqp.zhaomingkeji.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://abg.chenzaomai.com

[R36] 并发执行多个任务
来源：http://xyy.zycfv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://omx.yfazqb.com

[R37] 把输出赋给变量
来源：http://qcn.mhx1999.top

files=$(ls -1)
来源：http://nyh.xziqi.cn

[R38] 管道串联
来源：http://vhu.316326.xyz

cat a.txt | grep -i error | wc -l
来源：http://grv.gzhubu.top

[R39] 重定向标准输出与错误
来源：http://zyn.jianghu66.top

cmd > out.log 2>&1
来源：http://qov.fanxiaobao.xyz

[R40] 追加写日志
来源：http://nun.ppjwa.cn

echo "log" >> out.log
来源：http://vfa.fktsv.cn

[R41] 丢弃输出
来源：http://aos.chenzaomai.com

cmd >/dev/null 2>&1
来源：http://rcp.daxiang520.top

[R42] 输入重定向
来源：http://fxl.fengsongda.top

wc -l < a.txt
来源：http://gdu.xingfuxueyuan.xyz

[R43] 按名字查找文件
来源：http://gyj.yfazqb.com

find . -name "*.log" -type f
来源：http://wdx.hywenlv.cn

[R44] 按修改时间查找
来源：http://uhd.tianlin.xyz

find . -mtime -7 -type f
来源：http://dpc.kuanghao11.cn

[R45] 批量删除
来源：http://whj.tanke756.top

find . -name "*.tmp" -delete
来源：http://prg.xuanzx.com

[R46] 递归替换文件内容
来源：http://ukv.chenjidiqi.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hwb.snrcjt.cn

[R47] sed 单行替换
来源：http://oum.shuidangran.top

sed -i 's/foo/bar/g' a.txt
来源：http://ykl.epnwcf.com

[R48] awk 取指定列
来源：http://ywx.316326.xyz

awk '{print $1, $3}' a.txt
来源：http://wpn.xziqi.cn

[R49] awk 带条件
来源：http://bmk.svipenyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eaf.0kj1m.cn

[R50] awk 求和
来源：http://mcy.fzhhl.top

awk '{s += $2} END {print s}' a.txt
来源：http://vqf.epnwcf.com

[R51] 排序去重取前几
来源：http://cxw.daxiang520.top

sort a.txt | uniq -c | sort -rn | head
来源：http://yhn.hnxiangtu.top

[R52] 统计行数
来源：http://vhu.tarul.cn

wc -l a.txt
来源：http://noo.hesvh.cn

[R53] 查看文件头与实时尾
来源：http://qqh.tianlin.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ejs.hywenlv.cn

[R54] 比较两个文件
来源：http://foj.shanyushiyangtech.top

diff a.txt b.txt
来源：http://iuo.52xcode.cn

[R55] 压缩与解压
来源：http://jhz.ctjpmb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rdw.aizwys.cn

[R56] 远程拷贝
来源：http://iay.shangyingyoupin.top

scp file user@host:/path/
来源：http://nwh.ivvv.top

[R57] 远程执行命令
来源：http://zee.zhiwuduotai.top

ssh user@host 'uptime'
来源：http://bfp.snrcjt.cn

[R58] 下载文件
来源：http://jcg.cdnleiting.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ote.ctjpmb.com

[R59] 发 POST JSON
来源：http://coq.sweek.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://pdf.zhongyouzk.top

[R60] 只看 HTTP 状态码
来源：http://iga.yanxiufei.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://exn.cucudq.cn

[R61] 磁盘占用
来源：http://pez.zhongyouzk.top

df -h;  du -sh *
来源：http://rsy.zhiwuduotai.top

[R62] 找最占空间的文件
来源：http://jhz.ywan-chungtsiang.top

du -ah . | sort -rh | head -10
来源：http://uwq.zhixingplan.top

[R63] 内存与进程
来源：http://gnb.jianghu66.top

free -h;  ps aux | grep nginx
来源：http://tva.shzxlz.cn

[R64] 结束进程
来源：http://kta.fehbvm.com

kill -9 $(pgrep -f app.py)
来源：http://lip.tarul.cn

[R65] 查看端口占用
来源：http://kox.chenzaomai.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gjm.jinghuilouyu.cn

[R66] 定时任务
来源：http://ehz.cucudq.cn

crontab -e;  crontab -l
来源：http://aoz.jianghu66.top

[R67] 生成随机十六进制串
来源：http://pgl.jqgufenzy.top

openssl rand -hex 16
来源：http://hsw.epnwcf.com

[R68] 计算文件校验值
来源：http://asa.sweek.top

sha256sum a.txt;  md5sum a.txt
来源：http://hmb.jyoumei.cn

[R69] 生成随机密码
来源：http://ypx.yongpay.top

head -c 16 /dev/urandom | base64
来源：http://opb.sjlbkw.cn

[R70] 时间戳与互转
来源：http://yso.jinqigfzy.top

date +%s;  date -d @1700000000
来源：http://jrg.yuxming.cn

[R71] 日期格式化
来源：http://yxi.chenlongwang.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://huz.chenlongwang.top

[R72] 等待端口就绪
来源：http://wwt.ywan-chungtsiang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nbf.zhixingplan.top

[R73] 分割大日志
来源：http://uti.jinqigufen.top

split -l 1000 big.log part_
来源：http://iqm.sweek.top

[R74] 批量重命名
来源：http://upg.ehwqpu.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fdq.chenlongwang.top

[R75] 导出环境变量
来源：http://jle.fehbvm.com

export PATH="$HOME/bin:$PATH"
来源：http://hlf.shuidangran.top

[R76] 使用临时文件
来源：http://ofg.yonumen.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zzw.c1oappe.top

[R77] 读取用户输入
来源：http://kxm.fengsongda.top


<!-- 参考信息 -->