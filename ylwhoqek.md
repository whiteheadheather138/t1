代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://csu.hongshengwenyu.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wms.shanyushiyangtech.top

[Q39] 自连接（查上下级）
来源：http://vgw.xuanzx.com

SELECT e.name, m.name AS manager FROM employees e
来源：http://yae.dianchejie.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://pzc.xinyue.icu

[Q40] 交叉连接（笛卡尔积）
来源：http://qvo.aibaodan.cn

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wpu.tarul.cn

[Q41] 多表连接
来源：http://wuy.guannengcc.top

SELECT o.id, u.name, p.title FROM orders o
来源：http://bsa.yuanzhike.top

JOIN users u ON u.id = o.user_id
来源：http://kwx.guowangkeji.top

JOIN products p ON p.id = o.product_id;
来源：http://nyn.jyoumei.cn

[Q42] 连接条件附加过滤
来源：http://vjq.uphjek.com

SELECT u.name, o.amount FROM users u
来源：http://aww.zhixingplan.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://scg.daxiang520.top

[Q43] 标量子查询
来源：http://fnu.aizwys.cn

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://zxr.tian-w.cn

[Q44] IN 子查询
来源：http://iws.vehdjk.com

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://yds.cashguo.top

[Q45] EXISTS 判断存在
来源：http://phl.wangshuangyany.cn

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://cza.ehwqpu.com

[Q46] NOT EXISTS 判断不存在
来源：http://cgn.hnqzz.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://byz.yuxming.cn

[Q47] 与平均值比较
来源：http://lgn.c1oappe.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://oeo.jyoumei.cn

[Q48] CTE 公用表表达式
来源：http://cxe.guannengcc.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ahj.yj20258888.top

SELECT * FROM t WHERE c > 5;
来源：http://uxw.cheryme.top

[Q49] 更新单行
来源：http://sgn.jqgufenzy.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jbk.ybcxt.top

[Q50] 批量更新
来源：http://ozu.jiagoushi.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vxu.chenlongwang.top

[Q51] 用子查询更新
来源：http://vaw.yongpay.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://idh.jlsjyb.cn

[Q52] 删除指定行
来源：http://src.daria6918.cn

DELETE FROM users WHERE id = 10;
来源：http://dwi.birdmap.top

[Q53] 按条件删除
来源：http://ibq.zhixingplan.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wjh.bbcook.cn

[Q54] 清空表
来源：http://hua.shuidangran.top

TRUNCATE TABLE logs;
来源：http://tkr.yvedp.cn

[Q55] 排名（并列占位）
来源：http://alj.vehdjk.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wgk.0kj1m.cn

[Q56] 密集排名（并列不占位）
来源：http://bit.ehwqpu.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xgy.jiagoushi.top

[Q57] 行号
来源：http://mqs.cqqwz.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://ssv.shanyushiyangkeji.top

[Q58] 累计求和
来源：http://atm.ybcxt.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jpz.yangfankeji.com

[Q59] 分组内累计
来源：http://nkx.chenzaomai.com

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://dtr.nanxinkj.top

[Q60] 取上一行 / 下一行
来源：http://alz.316326.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gbs.dianchejie.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xke.birdmap.top

[Q61] 移动平均
来源：http://hkv.hesvh.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hmf.zhijiandao.cn

[Q62] 分组占比
来源：http://ioz.ehwqpu.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://vqu.yueranfly.top

[Q63] 开启事务
来源：http://sdw.cheryme.top

START TRANSACTION;                -- 或 BEGIN
来源：http://ctj.hammf.cn

[Q64] 提交事务
来源：http://gra.xingfuxueyuan.xyz

COMMIT;
来源：http://yeo.jinyuanbaomall.cn

[Q65] 回滚事务
来源：http://fug.cheryme.top

ROLLBACK;
来源：http://vdo.gotoacloud.top

[Q66] 行锁查询
来源：http://hdg.sjlbkw.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tbl.aibaodan.cn

[Q67] 设置隔离级别
来源：http://sqx.ctjpmb.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://brk.tian-w.cn

[Q68] 保存点
来源：http://vbz.wangshuangyany.cn

SAVEPOINT sp1;
来源：http://naj.birdmap.top

ROLLBACK TO sp1;
来源：http://hdy.vehdjk.com

[Q69] 查看执行计划
来源：http://qqm.wangshuangyany.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rpg.bbcook.cn

[Q70] 更新统计信息
来源：http://lma.sysykeji.top

ANALYZE TABLE users;
来源：http://xoz.shangyingyoupin.top

[Q71] 查看建表语句
来源：http://uuy.aizwys.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://eje.birdmap.top

[Q72] 查看索引
来源：http://vrv.dianchejie.cn

SHOW INDEX FROM users;
来源：http://krt.shangyingyoupin.top

[Q73] 查看表状态
来源：http://uax.svipenyu.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ovv.gzhubu.top

[Q74] 强制使用索引
来源：http://iph.epnwcf.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://nlt.xziqi.cn

[Q75] 日期格式化
来源：http://szd.vqdsnc.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ngq.9152youxi.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wsq.zdbjq.cn

[Q76] 按天统计
来源：http://hje.daxiang520.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://yfk.tianlin.xyz

[Q77] 时间加减
来源：http://eso.cheryme.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jgp.jqgfzy.top

[Q78] 当前时间
来源：http://gpm.svipenyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://osy.tian-w.cn

[Q79] 字符串拼接
来源：http://wcp.kuanghao11.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://eob.iojbl.cn

[Q80] 字符串截取
来源：http://msp.birdmap.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ltg.wangdashe.top

[Q81] 字符串替换
来源：http://btc.jinghuilouyu.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hbn.hammf.cn

[Q82] 字符长度与字节长度
来源：http://bwb.52xcode.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://fzr.birdmap.top

[Q83] 大小写转换
来源：http://mty.kuanghao11.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://voq.meibo888.top

[Q84] 去除首尾空格
来源：http://bop.mhx1999.top

SELECT TRIM(name) FROM users;
来源：http://lcu.yueranfly.top

[Q85] 数值取整
来源：http://uxq.jiagoushi.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xtk.andypj.xyz

[Q86] 读取 JSON 字段
来源：http://lsr.feifeiyinyue.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zod.zhengqikj.top

[Q87] JSON 字段做条件
来源：http://shb.zhongyouzk.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rij.hnqzz.top

[Q88] 行转列（条件聚合）
来源：http://vjd.316326.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fkd.hammf.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hqe.fzhhl.top

[Q89] 判断表是否存在
来源：http://uwe.jqgfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qvj.dashuyun.cn

[Q90] 生成序号列
来源：http://fer.yangfankeji.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ggm.jyoumei.cn

================================================================================
来源：http://dgv.cashguo.top

R. Bash 专题
来源：http://qap.jiagoushi.top

================================================================================
来源：http://elu.jinghuilouyu.cn

[R01] shebang 与严格模式
来源：http://ylc.wangshuangyany.cn

#!/usr/bin/env bash
来源：http://vtz.sxryk.cn

set -euo pipefail
来源：http://dhx.ydzc1.top

[R02] 变量赋值与使用
来源：http://dji.yj20258.top

name="Tom"; echo "$name"
来源：http://txw.gogol.net.cn

[R03] 只读变量
来源：http://szh.uphjek.com

readonly PI=3.14
来源：http://xzs.svipenyu.cn

[R04] 位置参数
来源：http://zzi.hywenlv.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://drx.hysaishi.cn

[R05] 参数默认值
来源：http://yqt.zdqjudy.top

name="${1:-default}"
来源：http://dix.ivvv.top

[R06] 判断命令是否存在
来源：http://lil.dashuyun.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cqm.jqgfzy.top

[R07] if 判断文件
来源：http://ykg.pengpengdd.cyou

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://weq.havefunace.top

[R08] 数值比较
来源：http://yrr.sweek.top

if (( a > b )); then echo "a 更大"; fi
来源：http://smc.cashguo.top

[R09] 字符串比较
来源：http://btc.ehwqpu.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://gkm.zhiwuduotai.top

[R10] 正则匹配
来源：http://kxx.feifeiyinyue.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://dkm.jinyuanbaomall.cn

[R11] case 多分支
来源：http://wxb.ppjwa.cn

case "$1" in
来源：http://hqu.fanxiaobao.xyz

start) echo "启动" ;;
来源：http://zlh.zycfv.cn

stop)  echo "停止" ;;
来源：http://peg.pengpengdd.cyou

*)     echo "未知命令" ;;
来源：http://gqh.sxryk.cn

esac
来源：http://asq.yj20258.top

[R12] for 遍历文件
来源：http://mkj.zhijiandao.cn

for f in *.txt; do echo "$f"; done
来源：http://ydf.0kj1m.cn

[R13] for 计数循环
来源：http://oyn.zhongyouzk.top

for i in {1..10}; do echo "$i"; done
来源：http://akl.hammf.cn

[R14] C 风格 for
来源：http://epn.zhijiandao.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ije.cdnleiting.top

[R15] while 逐行读文件
来源：http://hkq.sweek.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://rcl.sweek.top

[R16] until 等待条件
来源：http://lxf.iojbl.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://eri.zhengqikj.top

[R17] 数组定义与取值
来源：http://jhl.cdnleiting.top

arr=(a b c); echo "${arr[0]}"
来源：http://zjo.hfpthk.cn

[R18] 遍历数组
来源：http://rck.shangyingyoupin.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pjt.birdmap.top

[R19] 数组长度
来源：http://kyv.jinyuanbaomall.cn

echo "${#arr[@]}"
来源：http://wnz.ybcxt.top

[R20] 关联数组（字典）
来源：http://vgy.daria6918.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fos.feifeiyinyue.top

[R21] 字符串长度
来源：http://csx.hnqzz.top

echo "${#s}"
来源：http://nnj.c1oappe.top

[R22] 截取子串
来源：http://qeq.ywan-chungtsiang.top

echo "${s:0:5}"
来源：http://gdn.pycfn.com

[R23] 字符串替换
来源：http://nxb.jiagoushi.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vwt.ywan-chungtsiang.top

[R24] 大小写转换
来源：http://rpv.daria6918.cn

echo "${s^^}"; echo "${s,,}"
来源：http://bvn.fengsongda.top

[R25] 去后缀 / 去前缀
来源：http://sof.hammf.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cuh.shangyingyoupin.top

[R26] 命令替换
来源：http://csl.0kj1m.cn

now=$(date +%F); echo "$now"
来源：http://sge.guowangkeji.top

[R27] 算术展开
来源：http://jwk.jinqigufen.top

echo $((1 + 2 * 3))
来源：http://gqh.cdnleiting.top

[R28] 浮点运算
来源：http://wed.yj20258888.top

echo "scale=2; 10/3" | bc
来源：http://lbp.zhongyouzk.top

[R29] 定义函数
来源：http://fzz.cheryme.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://iec.tianlin.xyz

[R30] 函数返回状态码
来源：http://pmy.havefunace.top

f() { return 0; }; f || echo "失败了"
来源：http://vtz.shanyushiyangtech.top

[R31] 局部变量
来源：http://uqe.316326.xyz

f() { local x=1; echo "$x"; }
来源：http://jfl.hcnkem.com

[R32] 参数个数校验
来源：http://iht.hnxiangtu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hne.hammf.cn

[R33] 捕获错误并提示行号
来源：http://mdv.redwolf501.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tes.sufxvd.cn

[R34] 退出时清理
来源：http://jro.smart0.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://aeq.meibo888.top

[R35] 后台执行并等待
来源：http://gom.hnxiangtu.top

sleep 5 & pid=$!; wait "$pid"
来源：http://bek.shzxlz.cn

[R36] 并发执行多个任务
来源：http://wig.jinghuilouyu.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tje.guannengcc.top

[R37] 把输出赋给变量
来源：http://fbs.yj202588.top

files=$(ls -1)
来源：http://pby.dianchejie.cn

[R38] 管道串联
来源：http://dmw.wangshuangyany.cn

cat a.txt | grep -i error | wc -l
来源：http://lre.xinyue.icu

[R39] 重定向标准输出与错误
来源：http://ygq.chenlongwang.top

cmd > out.log 2>&1
来源：http://wuh.zhongyouzk.top

[R40] 追加写日志
来源：http://ywd.zhijiandao.cn

echo "log" >> out.log
来源：http://bvl.zhijiandao.cn

[R41] 丢弃输出
来源：http://sib.c1oappe.top

cmd >/dev/null 2>&1
来源：http://dce.jyoumei.cn

[R42] 输入重定向
来源：http://gze.fzhhl.top

wc -l < a.txt
来源：http://bts.hnqzz.top

[R43] 按名字查找文件
来源：http://oix.xingfuxueyuan.xyz

find . -name "*.log" -type f
来源：http://jjr.sjlbkw.cn

[R44] 按修改时间查找
来源：http://gnx.yfazqb.com

find . -mtime -7 -type f
来源：http://wim.ydjk.org.cn

[R45] 批量删除
来源：http://hun.sxryk.cn

find . -name "*.tmp" -delete
来源：http://bux.yangfankeji.com

[R46] 递归替换文件内容
来源：http://lof.chenjidiqi.icu

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cus.xuanzx.com

[R47] sed 单行替换
来源：http://yox.vehdjk.com

sed -i 's/foo/bar/g' a.txt
来源：http://yug.ybcxt.top

[R48] awk 取指定列
来源：http://xaz.xingfuxueyuan.xyz

awk '{print $1, $3}' a.txt
来源：http://ctm.shanyushiyangtech.top

[R49] awk 带条件
来源：http://cmb.sweek.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lqm.yanxiufei.cn

[R50] awk 求和
来源：http://hkm.sxryk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://cav.guowangkeji.top

[R51] 排序去重取前几
来源：http://prc.redwolf501.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cfn.zdbjq.cn

[R52] 统计行数
来源：http://iqj.ywan-chungtsiang.top

wc -l a.txt
来源：http://xwj.feifeiyinyue.top

[R53] 查看文件头与实时尾
来源：http://vhu.uphjek.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gfr.zhaomingkeji.xyz

[R54] 比较两个文件
来源：http://bqi.zhaomingkeji.xyz

diff a.txt b.txt
来源：http://pep.aizwys.cn

[R55] 压缩与解压
来源：http://yyx.xuetiantiany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qil.shuidangran.top

[R56] 远程拷贝
来源：http://hfw.bjfxy.top

scp file user@host:/path/
来源：http://ybx.guowangkeji.top

[R57] 远程执行命令
来源：http://agg.cdnleiting.top

ssh user@host 'uptime'
来源：http://pcy.chenlongwang.top

[R58] 下载文件
来源：http://nys.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eto.jqgufenzy.top

[R59] 发 POST JSON
来源：http://luu.nanxuanxn.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nir.sxryk.cn

[R60] 只看 HTTP 状态码
来源：http://vyh.havefunace.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://evj.fzhhl.top

[R61] 磁盘占用
来源：http://hbw.zdbjq.cn

df -h;  du -sh *
来源：http://pzn.ywan-chungtsiang.top

[R62] 找最占空间的文件
来源：http://act.0kj1m.cn

du -ah . | sort -rh | head -10
来源：http://jrn.jlsjyb.cn

[R63] 内存与进程
来源：http://qvr.svipenyu.cn

free -h;  ps aux | grep nginx
来源：http://vnv.jinyuanbaomall.cn

[R64] 结束进程
来源：http://vhh.xylfe.cn

kill -9 $(pgrep -f app.py)
来源：http://cey.vqdsnc.cn

[R65] 查看端口占用
来源：http://hiu.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ygy.hywenlv.cn

[R66] 定时任务
来源：http://jap.quarkkingdee.top

crontab -e;  crontab -l
来源：http://txl.jlsjyb.cn

[R67] 生成随机十六进制串
来源：http://ibh.c1oappe.top

openssl rand -hex 16
来源：http://ill.ehwqpu.com

[R68] 计算文件校验值
来源：http://vpq.jinyuanbaomall.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mhz.ywan-chungtsiang.top

[R69] 生成随机密码
来源：http://tch.zhengqikj.top

head -c 16 /dev/urandom | base64
来源：http://cne.tanke756.top

[R70] 时间戳与互转
来源：http://ava.sufxvd.cn

date +%s;  date -d @1700000000
来源：http://gdd.sysykeji.top

[R71] 日期格式化
来源：http://axz.dianchejie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ghv.gotoacloud.top

[R72] 等待端口就绪
来源：http://fck.gaohongyu789.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nbe.nanxinkj.top

[R73] 分割大日志
来源：http://iyv.sjlbkw.cn

split -l 1000 big.log part_
来源：http://phz.aibaodan.cn

[R74] 批量重命名
来源：http://bbt.xuanzx.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://twb.ydzc1.top

[R75] 导出环境变量
来源：http://hqn.shzxlz.cn

export PATH="$HOME/bin:$PATH"
来源：http://wcs.xuetiantiany.cn

[R76] 使用临时文件
来源：http://eif.chenjidiqi.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://asd.guowangkeji.top

[R77] 读取用户输入
来源：http://pun.zdbjq.cn

read -rp "请输入: " ans
来源：http://brn.jiagoushi.top

[R78] 交互式菜单
来源：http://grm.xuanzx.com

select opt in a b c; do echo "$opt"; break; done
来源：http://etn.zhengqikj.top

[R79] 解析命令行选项
来源：http://npd.cdnleiting.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eca.daxiang520.top

[R80] 查看脚本执行耗时
来源：http://wvo.yangfankeji.com

time ./run.sh
来源：http://ijn.ybcxt.top

================================================================================
来源：http://rce.ivvv.top

S. C / C++ 专题
来源：http://kys.chenzaomai.com

================================================================================
来源：http://lho.hfpthk.cn

[S01] C：Hello World
来源：http://jmu.sufxvd.cn

#include <stdio.h>
来源：http://qvw.zdbjq.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xxe.birdmap.top

[S02] C：变量与格式化输出
来源：http://otg.jinqigfzy.top

int a = 10; printf("%d\n", a);
来源：http://opl.smart0.xyz

[S03] C：读入整数
来源：http://wsy.52xcode.cn

int x; scanf("%d", &x);
来源：http://yoz.hnxiangtu.top

[S04] C：字符串复制
来源：http://eud.quarkkingdee.top

char dst[32]; strcpy(dst, "hi");
来源：http://ffl.iojbl.cn

[S05] C：字符串长度
来源：http://lyi.zycfv.cn

strlen(s)
来源：http://xnx.jinqigfzy.top

[S06] C：字符串比较
来源：http://vum.zhijiandao.cn

strcmp(a, b) == 0
来源：http://ehw.mhx1999.top

[S07] C：数组遍历求和
来源：http://nbi.yj20258.top


<!-- 参考信息 -->