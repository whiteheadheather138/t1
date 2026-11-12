代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://aiq.wangdashe.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://jah.xuetiantiany.cn

[Q39] 自连接（查上下级）
来源：http://qgw.ehwqpu.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://fhd.shuidangran.top

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://lig.mhx1999.top

[Q40] 交叉连接（笛卡尔积）
来源：http://cza.birdmap.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://tkw.shzxlz.cn

[Q41] 多表连接
来源：http://svw.andypj.xyz

SELECT o.id, u.name, p.title FROM orders o
来源：http://bsn.pengpengdd.cyou

JOIN users u ON u.id = o.user_id
来源：http://ohd.nwbrower.top

JOIN products p ON p.id = o.product_id;
来源：http://dli.tanke756.top

[Q42] 连接条件附加过滤
来源：http://qmq.gaohongyu789.top

SELECT u.name, o.amount FROM users u
来源：http://aio.zhijiandao.cn

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://sbl.epnwcf.com

[Q43] 标量子查询
来源：http://lcl.sysykeji.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hlq.yj202588.top

[Q44] IN 子查询
来源：http://sbg.haohaochexian.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ale.yfazqb.com

[Q45] EXISTS 判断存在
来源：http://qlq.jiagoushi.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zsi.hnqzz.top

[Q46] NOT EXISTS 判断不存在
来源：http://lxi.chenjidiqi.icu

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://yyk.cheryme.top

[Q47] 与平均值比较
来源：http://hkq.chenlongwang.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://iob.chenzaomai.com

[Q48] CTE 公用表表达式
来源：http://lpk.52xcode.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://qgy.cashguo.top

SELECT * FROM t WHERE c > 5;
来源：http://gvp.vqdsnc.cn

[Q49] 更新单行
来源：http://ejy.yj202588.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://oea.uphjek.com

[Q50] 批量更新
来源：http://fqy.xziqi.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://xeu.gogol.net.cn

[Q51] 用子查询更新
来源：http://vbi.ivvv.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://pzx.0kj1m.cn

[Q52] 删除指定行
来源：http://zfn.birdmap.top

DELETE FROM users WHERE id = 10;
来源：http://qzu.sweek.top

[Q53] 按条件删除
来源：http://uvq.chenzaomai.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://usr.iojbl.cn

[Q54] 清空表
来源：http://pnh.zdqjudy.top

TRUNCATE TABLE logs;
来源：http://trp.sysykeji.top

[Q55] 排名（并列占位）
来源：http://yfk.dianchejie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jge.zhoulong.xyz

[Q56] 密集排名（并列不占位）
来源：http://wew.fanxiaobao.xyz

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mcc.yangfankeji.com

[Q57] 行号
来源：http://xwc.vqdsnc.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://kgk.jianghu66.top

[Q58] 累计求和
来源：http://lkw.cdnleiting.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yin.hnqzz.top

[Q59] 分组内累计
来源：http://juy.jianghu66.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pfq.quarkkingdee.top

[Q60] 取上一行 / 下一行
来源：http://pzs.sxryk.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://vqf.guannengcc.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://rff.ivvv.top

[Q61] 移动平均
来源：http://sfx.hfpthk.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://btw.andypj.xyz

[Q62] 分组占比
来源：http://nkl.redwolf501.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://dui.jiagoushi.top

[Q63] 开启事务
来源：http://pvm.haohaochexian.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hll.tianlin.xyz

[Q64] 提交事务
来源：http://uqy.sjlbkw.cn

COMMIT;
来源：http://wyt.zhiwuduotai.top

[Q65] 回滚事务
来源：http://hxz.aibaodan.cn

ROLLBACK;
来源：http://txn.zhaomingkeji.xyz

[Q66] 行锁查询
来源：http://dfp.iojbl.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bqs.chenjidiqi.icu

[Q67] 设置隔离级别
来源：http://nno.ydzc1.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zkk.nwbrower.top

[Q68] 保存点
来源：http://xpo.nanxuanxn.top

SAVEPOINT sp1;
来源：http://rgo.zhijiandao.cn

ROLLBACK TO sp1;
来源：http://eac.shangyingyoupin.top

[Q69] 查看执行计划
来源：http://del.yj202588.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pnf.yangfankeji.com

[Q70] 更新统计信息
来源：http://qvr.cdnleiting.top

ANALYZE TABLE users;
来源：http://gkj.0kj1m.cn

[Q71] 查看建表语句
来源：http://udt.zhijiandao.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://cxc.dianchejie.cn

[Q72] 查看索引
来源：http://vvn.gaohongyu789.top

SHOW INDEX FROM users;
来源：http://omw.tian-w.cn

[Q73] 查看表状态
来源：http://svq.jqgfzy.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ywf.316326.xyz

[Q74] 强制使用索引
来源：http://gsk.daxiang520.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tqt.zhaomingkeji.xyz

[Q75] 日期格式化
来源：http://uys.iojbl.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://qlj.haohaochexian.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://yqw.52xcode.cn

[Q76] 按天统计
来源：http://mwk.bjfxy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://tfz.jqgufenzy.top

[Q77] 时间加减
来源：http://wgd.cashguo.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://gvh.pycfn.com

[Q78] 当前时间
来源：http://ksg.iojbl.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://cxz.hcnkem.com

[Q79] 字符串拼接
来源：http://eni.chenlongwang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ayq.yanxiufei.cn

[Q80] 字符串截取
来源：http://mmh.sxryk.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ajy.zhiwuduotai.top

[Q81] 字符串替换
来源：http://ywu.jyoumei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://vij.zycfv.cn

[Q82] 字符长度与字节长度
来源：http://dtr.jinqigufen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ldy.shanyushiyangtech.top

[Q83] 大小写转换
来源：http://ecs.cashguo.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kfd.hnqzz.top

[Q84] 去除首尾空格
来源：http://ivq.fzhhl.top

SELECT TRIM(name) FROM users;
来源：http://ytk.316326.xyz

[Q85] 数值取整
来源：http://kcj.havefunace.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://tkb.ehwqpu.com

[Q86] 读取 JSON 字段
来源：http://yii.wangdashe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://bqk.zhaomingkeji.xyz

[Q87] JSON 字段做条件
来源：http://nbl.yongpay.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gsa.dianchejie.cn

[Q88] 行转列（条件聚合）
来源：http://nyd.sjlbkw.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ype.jinqigfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hui.xziqi.cn

[Q89] 判断表是否存在
来源：http://ddx.hnqzz.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://eou.hywenlv.cn

[Q90] 生成序号列
来源：http://rfk.zycfv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://kgh.shanyushiyangkeji.top

================================================================================
来源：http://osu.yonumen.top

R. Bash 专题
来源：http://rja.daria6918.cn

================================================================================
来源：http://bsu.cqqwz.cn

[R01] shebang 与严格模式
来源：http://ufr.9152youxi.cn

#!/usr/bin/env bash
来源：http://qnj.jqgufenzy.top

set -euo pipefail
来源：http://evw.gzhubu.top

[R02] 变量赋值与使用
来源：http://mpr.shanyushiyangkeji.top

name="Tom"; echo "$name"
来源：http://rsq.hesvh.cn

[R03] 只读变量
来源：http://orn.52xcode.cn

readonly PI=3.14
来源：http://fxn.zhoulong.xyz

[R04] 位置参数
来源：http://sok.pengpengdd.cyou

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wbi.fzhhl.top

[R05] 参数默认值
来源：http://dbt.zdqjudy.top

name="${1:-default}"
来源：http://ldt.ybcxt.top

[R06] 判断命令是否存在
来源：http://fmp.52xcode.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tbd.andypj.xyz

[R07] if 判断文件
来源：http://wxu.zhiwuduotai.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://nls.svipenyu.cn

[R08] 数值比较
来源：http://uxl.sysykeji.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qmm.xingfuxueyuan.xyz

[R09] 字符串比较
来源：http://jnf.sxryk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bez.zdqjudy.top

[R10] 正则匹配
来源：http://bex.gotoacloud.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ozr.tian-w.cn

[R11] case 多分支
来源：http://wfk.sysykeji.top

case "$1" in
来源：http://npd.jianghu66.top

start) echo "启动" ;;
来源：http://rjz.yuxming.cn

stop)  echo "停止" ;;
来源：http://mwd.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://bxp.hongshengwenyu.top

esac
来源：http://olg.fktsv.cn

[R12] for 遍历文件
来源：http://dhx.fzhhl.top

for f in *.txt; do echo "$f"; done
来源：http://dwi.ywan-chungtsiang.top

[R13] for 计数循环
来源：http://xbk.bjfxy.top

for i in {1..10}; do echo "$i"; done
来源：http://jxr.gzhubu.top

[R14] C 风格 for
来源：http://eip.sysykeji.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vqe.ppjwa.cn

[R15] while 逐行读文件
来源：http://vtt.tarul.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mxw.guowangkeji.top

[R16] until 等待条件
来源：http://bax.jqgufenzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vet.gzhubu.top

[R17] 数组定义与取值
来源：http://xfw.c1oappe.top

arr=(a b c); echo "${arr[0]}"
来源：http://ysc.haohaochexian.top

[R18] 遍历数组
来源：http://fez.chenjidiqi.icu

for x in "${arr[@]}"; do echo "$x"; done
来源：http://cay.jinqigufen.top

[R19] 数组长度
来源：http://eha.bbcook.cn

echo "${#arr[@]}"
来源：http://mzn.fzhhl.top

[R20] 关联数组（字典）
来源：http://lia.yuanzhike.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://sgv.gotoacloud.top

[R21] 字符串长度
来源：http://cpl.aibaodan.cn

echo "${#s}"
来源：http://sah.zhixingplan.top

[R22] 截取子串
来源：http://fjg.nwbrower.top

echo "${s:0:5}"
来源：http://ygv.316326.xyz

[R23] 字符串替换
来源：http://khi.aizwys.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vok.redwolf501.top

[R24] 大小写转换
来源：http://hpw.tanke756.top

echo "${s^^}"; echo "${s,,}"
来源：http://mck.jianghu66.top

[R25] 去后缀 / 去前缀
来源：http://zfv.svipenyu.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://zss.cheryme.top

[R26] 命令替换
来源：http://vuy.gaohongyu789.top

now=$(date +%F); echo "$now"
来源：http://bvc.ivvv.top

[R27] 算术展开
来源：http://hwl.zhixingplan.top

echo $((1 + 2 * 3))
来源：http://ojy.yj20258.top

[R28] 浮点运算
来源：http://fmm.hammf.cn

echo "scale=2; 10/3" | bc
来源：http://fba.sxryk.cn

[R29] 定义函数
来源：http://fth.jyoumei.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://sqt.xziqi.cn

[R30] 函数返回状态码
来源：http://rax.yj20258.top

f() { return 0; }; f || echo "失败了"
来源：http://rcp.yueranfly.top

[R31] 局部变量
来源：http://mdh.vqdsnc.cn

f() { local x=1; echo "$x"; }
来源：http://wyp.bbcook.cn

[R32] 参数个数校验
来源：http://jyi.ydjk.org.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mkj.yonumen.top

[R33] 捕获错误并提示行号
来源：http://sms.yuxming.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://iqa.fzhhl.top

[R34] 退出时清理
来源：http://iws.0kj1m.cn

trap 'rm -f "$tmp"' EXIT
来源：http://hwa.uphjek.com

[R35] 后台执行并等待
来源：http://bpf.zhongyouzk.top

sleep 5 & pid=$!; wait "$pid"
来源：http://lei.9152youxi.cn

[R36] 并发执行多个任务
来源：http://pyk.jinqigfzy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uqv.ydjk.org.cn

[R37] 把输出赋给变量
来源：http://tuo.gogol.net.cn

files=$(ls -1)
来源：http://icj.gaohongyu789.top

[R38] 管道串联
来源：http://xrq.yongpay.top

cat a.txt | grep -i error | wc -l
来源：http://tnw.ctjpmb.com

[R39] 重定向标准输出与错误
来源：http://ock.c1oappe.top

cmd > out.log 2>&1
来源：http://hrl.sxryk.cn

[R40] 追加写日志
来源：http://vid.quarkkingdee.top

echo "log" >> out.log
来源：http://nlo.andypj.xyz

[R41] 丢弃输出
来源：http://nxd.xingfuxueyuan.xyz

cmd >/dev/null 2>&1
来源：http://rxv.ctjpmb.com

[R42] 输入重定向
来源：http://qmt.ehwqpu.com

wc -l < a.txt
来源：http://dqp.hcnkem.com

[R43] 按名字查找文件
来源：http://swv.sxryk.cn

find . -name "*.log" -type f
来源：http://qhs.zhoulong.xyz

[R44] 按修改时间查找
来源：http://pca.vqdsnc.cn

find . -mtime -7 -type f
来源：http://ztb.tanke756.top

[R45] 批量删除
来源：http://nnb.cdnleiting.top

find . -name "*.tmp" -delete
来源：http://lmt.hammf.cn

[R46] 递归替换文件内容
来源：http://mcs.c1oappe.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ibk.iojbl.cn

[R47] sed 单行替换
来源：http://mbu.jinqigfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://bep.jinghuilouyu.cn

[R48] awk 取指定列
来源：http://xgf.chenlongwang.top

awk '{print $1, $3}' a.txt
来源：http://hfi.dianchejie.cn

[R49] awk 带条件
来源：http://vph.tian-w.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gna.zhaomingkeji.xyz

[R50] awk 求和
来源：http://hny.yj20258888.top

awk '{s += $2} END {print s}' a.txt
来源：http://env.aibaodan.cn

[R51] 排序去重取前几
来源：http://vlt.gaohongyu789.top

sort a.txt | uniq -c | sort -rn | head
来源：http://gqn.cucudq.cn

[R52] 统计行数
来源：http://ioh.hysaishi.cn

wc -l a.txt
来源：http://cnp.jinqigfzy.top

[R53] 查看文件头与实时尾
来源：http://tli.9152youxi.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oeh.redwolf501.top

[R54] 比较两个文件
来源：http://ckv.ppjwa.cn

diff a.txt b.txt
来源：http://kih.feifeiyinyue.top

[R55] 压缩与解压
来源：http://xbo.svipenyu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lnw.xingfuxueyuan.xyz

[R56] 远程拷贝
来源：http://xpe.0kj1m.cn

scp file user@host:/path/
来源：http://mlp.hcnkem.com

[R57] 远程执行命令
来源：http://ctm.kuanghao11.cn

ssh user@host 'uptime'
来源：http://kll.daxiang520.top

[R58] 下载文件
来源：http://tkd.daria6918.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vvf.jyoumei.cn

[R59] 发 POST JSON
来源：http://gux.ivvv.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qzl.haohaochexian.top

[R60] 只看 HTTP 状态码
来源：http://vel.52xcode.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rte.fzhhl.top

[R61] 磁盘占用
来源：http://ohn.hcnkem.com

df -h;  du -sh *
来源：http://zoo.zhijiandao.cn

[R62] 找最占空间的文件
来源：http://nug.zhijiandao.cn

du -ah . | sort -rh | head -10
来源：http://mcu.sxryk.cn

[R63] 内存与进程
来源：http://jwp.cashguo.top

free -h;  ps aux | grep nginx
来源：http://uwg.zdbjq.cn

[R64] 结束进程
来源：http://ope.cheryme.top

kill -9 $(pgrep -f app.py)
来源：http://wyj.ydzc1.top

[R65] 查看端口占用
来源：http://vbr.zhongyouzk.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://aff.cucudq.cn

[R66] 定时任务
来源：http://luo.jlsjyb.cn

crontab -e;  crontab -l
来源：http://mue.ehwqpu.com

[R67] 生成随机十六进制串
来源：http://pfg.yj202588.top

openssl rand -hex 16
来源：http://ujo.ydjk.org.cn

[R68] 计算文件校验值
来源：http://apt.gzhubu.top

sha256sum a.txt;  md5sum a.txt
来源：http://jiy.gogol.net.cn

[R69] 生成随机密码
来源：http://znt.uphjek.com

head -c 16 /dev/urandom | base64
来源：http://eqi.shzxlz.cn

[R70] 时间戳与互转
来源：http://eig.vqdsnc.cn

date +%s;  date -d @1700000000
来源：http://yqc.jqgufenzy.top

[R71] 日期格式化
来源：http://vpp.tarul.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ndc.zhoulong.xyz

[R72] 等待端口就绪
来源：http://mta.fengsongda.top

until nc -z localhost 3306; do sleep 1; done
来源：http://kvw.cdnleiting.top

[R73] 分割大日志
来源：http://zox.chenjidiqi.icu

split -l 1000 big.log part_
来源：http://ezp.redwolf501.top

[R74] 批量重命名
来源：http://qyd.meibo888.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xyb.yj20258888.top

[R75] 导出环境变量
来源：http://udk.daria6918.cn

export PATH="$HOME/bin:$PATH"
来源：http://vgn.yueranfly.top

[R76] 使用临时文件
来源：http://vda.shangyingyoupin.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jun.sweek.top

[R77] 读取用户输入
来源：http://zfl.tian-w.cn

read -rp "请输入: " ans
来源：http://xmo.cucudq.cn

[R78] 交互式菜单
来源：http://dob.jinghuilouyu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hwb.redwolf501.top

[R79] 解析命令行选项
来源：http://gph.uphjek.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qnn.cucudq.cn

[R80] 查看脚本执行耗时
来源：http://jgw.jqgufenzy.top

time ./run.sh
来源：http://zzb.gaohongyu789.top

================================================================================
来源：http://psm.quarkkingdee.top

S. C / C++ 专题
来源：http://aux.vqdsnc.cn

================================================================================
来源：http://wog.yueranfly.top

[S01] C：Hello World
来源：http://vfc.ivvv.top

#include <stdio.h>
来源：http://fhq.mhx1999.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://rcz.hfpthk.cn

[S02] C：变量与格式化输出
来源：http://ole.fehbvm.com

int a = 10; printf("%d\n", a);
来源：http://cqe.fehbvm.com

[S03] C：读入整数
来源：http://bkm.zhiwuduotai.top

int x; scanf("%d", &x);
来源：http://mvk.yj202588.top

[S04] C：字符串复制
来源：http://csr.ybcxt.top

char dst[32]; strcpy(dst, "hi");
来源：http://evs.yuanzhike.top

[S05] C：字符串长度
来源：http://jty.hesvh.cn

strlen(s)
来源：http://fjd.zhengqikj.top

[S06] C：字符串比较
来源：http://rqd.jqgufenzy.top

strcmp(a, b) == 0
来源：http://xpv.jqgufenzy.top

[S07] C：数组遍历求和
来源：http://yau.jianghu66.top


<!-- 参考信息 -->