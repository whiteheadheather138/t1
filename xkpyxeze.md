代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://zuj.cashguo.top

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://luz.andypj.xyz

[Q39] 自连接（查上下级）
来源：http://kin.yj202588.top

SELECT e.name, m.name AS manager FROM employees e
来源：http://umr.yvedp.cn

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wef.xingfuxueyuan.xyz

[Q40] 交叉连接（笛卡尔积）
来源：http://gjo.nanxinkj.top

SELECT * FROM colors CROSS JOIN sizes;
来源：http://ijs.quarkkingdee.top

[Q41] 多表连接
来源：http://nxo.pengpengdd.cyou

SELECT o.id, u.name, p.title FROM orders o
来源：http://ani.yonumen.top

JOIN users u ON u.id = o.user_id
来源：http://jnc.fanxiaobao.xyz

JOIN products p ON p.id = o.product_id;
来源：http://cav.jlsjyb.cn

[Q42] 连接条件附加过滤
来源：http://jrr.xziqi.cn

SELECT u.name, o.amount FROM users u
来源：http://bav.zhixingplan.top

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://uky.zycfv.cn

[Q43] 标量子查询
来源：http://fyo.yj20258.top

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://aik.aizwys.cn

[Q44] IN 子查询
来源：http://hzb.hesvh.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://ltb.zhijiandao.cn

[Q45] EXISTS 判断存在
来源：http://qdt.ywan-chungtsiang.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zjl.zhiwuduotai.top

[Q46] NOT EXISTS 判断不存在
来源：http://tra.guannengcc.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zgu.zycfv.cn

[Q47] 与平均值比较
来源：http://pmn.sxryk.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://nxc.birdmap.top

[Q48] CTE 公用表表达式
来源：http://dob.sufxvd.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wdz.cqqwz.cn

SELECT * FROM t WHERE c > 5;
来源：http://yxo.pengpengdd.cyou

[Q49] 更新单行
来源：http://voo.nanxuanxn.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://xtp.ybcxt.top

[Q50] 批量更新
来源：http://dun.svipenyu.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://izr.zhengqikj.top

[Q51] 用子查询更新
来源：http://oib.zhijiandao.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://njm.guowangkeji.top

[Q52] 删除指定行
来源：http://xub.cqqwz.cn

DELETE FROM users WHERE id = 10;
来源：http://ufc.ybcxt.top

[Q53] 按条件删除
来源：http://itl.pycfn.com

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://icy.feifeiyinyue.top

[Q54] 清空表
来源：http://pdv.sysykeji.top

TRUNCATE TABLE logs;
来源：http://dgo.shangyingyoupin.top

[Q55] 排名（并列占位）
来源：http://bjn.jinyuanbaomall.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yvz.yongpay.top

[Q56] 密集排名（并列不占位）
来源：http://euq.ctjpmb.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xdr.hcnkem.com

[Q57] 行号
来源：http://bxb.zhengqikj.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://twq.jinghuilouyu.cn

[Q58] 累计求和
来源：http://jea.xingfuxueyuan.xyz

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mbx.gzhubu.top

[Q59] 分组内累计
来源：http://vyi.feifeiyinyue.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://qly.zdqjudy.top

[Q60] 取上一行 / 下一行
来源：http://peu.fehbvm.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wrz.epnwcf.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lmw.fanxiaobao.xyz

[Q61] 移动平均
来源：http://uel.snrcjt.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://awm.ydzc1.top

[Q62] 分组占比
来源：http://uev.uphjek.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zpb.tarul.cn

[Q63] 开启事务
来源：http://ukq.chenzaomai.com

START TRANSACTION;                -- 或 BEGIN
来源：http://las.zhiwuduotai.top

[Q64] 提交事务
来源：http://msk.aibaodan.cn

COMMIT;
来源：http://qod.bbcook.cn

[Q65] 回滚事务
来源：http://jgm.zhongyouzk.top

ROLLBACK;
来源：http://gdt.tian-w.cn

[Q66] 行锁查询
来源：http://fow.haohaochexian.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://clu.epnwcf.com

[Q67] 设置隔离级别
来源：http://skt.52xcode.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://fdt.bbcook.cn

[Q68] 保存点
来源：http://mzg.nanxinkj.top

SAVEPOINT sp1;
来源：http://tqm.zdbjq.cn

ROLLBACK TO sp1;
来源：http://ssw.hywenlv.cn

[Q69] 查看执行计划
来源：http://euq.yanxiufei.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://aei.fehbvm.com

[Q70] 更新统计信息
来源：http://jsp.jiagoushi.top

ANALYZE TABLE users;
来源：http://oyr.jinghuilouyu.cn

[Q71] 查看建表语句
来源：http://esn.0kj1m.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nxp.fzhhl.top

[Q72] 查看索引
来源：http://xxc.cashguo.top

SHOW INDEX FROM users;
来源：http://jua.zhengqikj.top

[Q73] 查看表状态
来源：http://htv.9152youxi.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://gzk.uphjek.com

[Q74] 强制使用索引
来源：http://lxg.nwbrower.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://unq.cucudq.cn

[Q75] 日期格式化
来源：http://okj.tianlin.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://gil.aibaodan.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://oqz.yangfankeji.com

[Q76] 按天统计
来源：http://zvr.gogol.net.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://nog.feifeiyinyue.top

[Q77] 时间加减
来源：http://esl.ydzc1.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://api.hfpthk.cn

[Q78] 当前时间
来源：http://dqb.epnwcf.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://scb.xziqi.cn

[Q79] 字符串拼接
来源：http://sox.sufxvd.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://xal.zdqjudy.top

[Q80] 字符串截取
来源：http://ufw.zdqjudy.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://res.jyoumei.cn

[Q81] 字符串替换
来源：http://vod.ydjk.org.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iif.andypj.xyz

[Q82] 字符长度与字节长度
来源：http://ffk.nanxuanxn.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rvi.feifeiyinyue.top

[Q83] 大小写转换
来源：http://hnf.316326.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fbp.aibaodan.cn

[Q84] 去除首尾空格
来源：http://ory.316326.xyz

SELECT TRIM(name) FROM users;
来源：http://zne.redwolf501.top

[Q85] 数值取整
来源：http://cjn.haohaochexian.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vvv.wangdashe.top

[Q86] 读取 JSON 字段
来源：http://ozf.xuanzx.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mxv.cucudq.cn

[Q87] JSON 字段做条件
来源：http://xsf.ppjwa.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://zmv.sufxvd.cn

[Q88] 行转列（条件聚合）
来源：http://gzc.uphjek.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mbz.zhoulong.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kgq.fanxiaobao.xyz

[Q89] 判断表是否存在
来源：http://tky.tarul.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://pky.zhengqikj.top

[Q90] 生成序号列
来源：http://hmu.jinghuilouyu.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://gzt.yj20258888.top

================================================================================
来源：http://lkz.iojbl.cn

R. Bash 专题
来源：http://hhm.fktsv.cn

================================================================================
来源：http://fjj.hfpthk.cn

[R01] shebang 与严格模式
来源：http://tdl.svipenyu.cn

#!/usr/bin/env bash
来源：http://bjd.aizwys.cn

set -euo pipefail
来源：http://yzf.aibaodan.cn

[R02] 变量赋值与使用
来源：http://yez.shzxlz.cn

name="Tom"; echo "$name"
来源：http://ylb.hfpthk.cn

[R03] 只读变量
来源：http://lak.shanyushiyangtech.top

readonly PI=3.14
来源：http://skp.yvedp.cn

[R04] 位置参数
来源：http://vqt.cucudq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://meu.xziqi.cn

[R05] 参数默认值
来源：http://azt.tianlin.xyz

name="${1:-default}"
来源：http://yqe.zhengqikj.top

[R06] 判断命令是否存在
来源：http://ezu.yuanzhike.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jek.vehdjk.com

[R07] if 判断文件
来源：http://oyb.fehbvm.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://gjh.tianlin.xyz

[R08] 数值比较
来源：http://kca.birdmap.top

if (( a > b )); then echo "a 更大"; fi
来源：http://pyi.zhengqikj.top

[R09] 字符串比较
来源：http://aqr.zdqjudy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nvt.ydjk.org.cn

[R10] 正则匹配
来源：http://ovn.zhaomingkeji.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pll.ydzc1.top

[R11] case 多分支
来源：http://nbk.zhixingplan.top

case "$1" in
来源：http://grd.bjfxy.top

start) echo "启动" ;;
来源：http://ioc.ctjpmb.com

stop)  echo "停止" ;;
来源：http://tbg.sxryk.cn

*)     echo "未知命令" ;;
来源：http://wmx.yuanzhike.top

esac
来源：http://zmq.daria6918.cn

[R12] for 遍历文件
来源：http://kxx.tian-w.cn

for f in *.txt; do echo "$f"; done
来源：http://zyp.pengpengdd.cyou

[R13] for 计数循环
来源：http://xlp.tanke756.top

for i in {1..10}; do echo "$i"; done
来源：http://kaq.sweek.top

[R14] C 风格 for
来源：http://vfo.fengsongda.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://msz.nanxuanxn.top

[R15] while 逐行读文件
来源：http://nbf.dianchejie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sop.wangdashe.top

[R16] until 等待条件
来源：http://ylc.hammf.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mpr.wangdashe.top

[R17] 数组定义与取值
来源：http://pyw.ivvv.top

arr=(a b c); echo "${arr[0]}"
来源：http://mwg.tian-w.cn

[R18] 遍历数组
来源：http://leu.zhijiandao.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://gxr.9152youxi.cn

[R19] 数组长度
来源：http://utl.yongpay.top

echo "${#arr[@]}"
来源：http://wej.yj202588.top

[R20] 关联数组（字典）
来源：http://fba.chenjidiqi.icu

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://msc.cdnleiting.top

[R21] 字符串长度
来源：http://ehi.zhixingplan.top

echo "${#s}"
来源：http://dpi.wangshuangyany.cn

[R22] 截取子串
来源：http://gru.bjfxy.top

echo "${s:0:5}"
来源：http://aow.zhiwuduotai.top

[R23] 字符串替换
来源：http://ctu.shanyushiyangtech.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ave.yonumen.top

[R24] 大小写转换
来源：http://wrl.yuanzhike.top

echo "${s^^}"; echo "${s,,}"
来源：http://vzc.svipenyu.cn

[R25] 去后缀 / 去前缀
来源：http://pgp.jinyuanbaomall.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://pvk.ehwqpu.com

[R26] 命令替换
来源：http://zah.c1oappe.top

now=$(date +%F); echo "$now"
来源：http://ldl.shanyushiyangkeji.top

[R27] 算术展开
来源：http://lfa.9152youxi.cn

echo $((1 + 2 * 3))
来源：http://lie.chenjidiqi.icu

[R28] 浮点运算
来源：http://frm.aizwys.cn

echo "scale=2; 10/3" | bc
来源：http://odt.shanyushiyangtech.top

[R29] 定义函数
来源：http://dbg.52xcode.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zms.epnwcf.com

[R30] 函数返回状态码
来源：http://zwx.snrcjt.cn

f() { return 0; }; f || echo "失败了"
来源：http://zmy.sxryk.cn

[R31] 局部变量
来源：http://ahv.zycfv.cn

f() { local x=1; echo "$x"; }
来源：http://qlh.ywan-chungtsiang.top

[R32] 参数个数校验
来源：http://kjo.xylfe.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://dug.yonumen.top

[R33] 捕获错误并提示行号
来源：http://rfz.sufxvd.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ghw.jqgufenzy.top

[R34] 退出时清理
来源：http://qdj.yueranfly.top

trap 'rm -f "$tmp"' EXIT
来源：http://qye.ybcxt.top

[R35] 后台执行并等待
来源：http://wmg.yongpay.top

sleep 5 & pid=$!; wait "$pid"
来源：http://fvb.epnwcf.com

[R36] 并发执行多个任务
来源：http://pua.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://edi.haohaochexian.top

[R37] 把输出赋给变量
来源：http://qnk.yj20258.top

files=$(ls -1)
来源：http://pkd.wangdashe.top

[R38] 管道串联
来源：http://mts.shzxlz.cn

cat a.txt | grep -i error | wc -l
来源：http://kzi.jinqigufen.top

[R39] 重定向标准输出与错误
来源：http://nas.tianlin.xyz

cmd > out.log 2>&1
来源：http://lak.tarul.cn

[R40] 追加写日志
来源：http://wba.xylfe.cn

echo "log" >> out.log
来源：http://bpm.hesvh.cn

[R41] 丢弃输出
来源：http://mwe.nanxuanxn.top

cmd >/dev/null 2>&1
来源：http://fnu.havefunace.top

[R42] 输入重定向
来源：http://exf.zycfv.cn

wc -l < a.txt
来源：http://elf.yfazqb.com

[R43] 按名字查找文件
来源：http://jzv.redwolf501.top

find . -name "*.log" -type f
来源：http://tgr.daria6918.cn

[R44] 按修改时间查找
来源：http://wno.hesvh.cn

find . -mtime -7 -type f
来源：http://kvw.hammf.cn

[R45] 批量删除
来源：http://uap.uphjek.com

find . -name "*.tmp" -delete
来源：http://xgk.andypj.xyz

[R46] 递归替换文件内容
来源：http://rxt.aizwys.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hxq.yj20258888.top

[R47] sed 单行替换
来源：http://xzi.kuanghao11.cn

sed -i 's/foo/bar/g' a.txt
来源：http://uai.fanxiaobao.xyz

[R48] awk 取指定列
来源：http://wky.birdmap.top

awk '{print $1, $3}' a.txt
来源：http://ged.ydjk.org.cn

[R49] awk 带条件
来源：http://qxz.zycfv.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ewm.yongpay.top

[R50] awk 求和
来源：http://hnl.yuanzhike.top

awk '{s += $2} END {print s}' a.txt
来源：http://ybn.vqdsnc.cn

[R51] 排序去重取前几
来源：http://fbt.shanyushiyangtech.top

sort a.txt | uniq -c | sort -rn | head
来源：http://nnb.52xcode.cn

[R52] 统计行数
来源：http://lin.xuetiantiany.cn

wc -l a.txt
来源：http://uhu.zhengqikj.top

[R53] 查看文件头与实时尾
来源：http://kgy.zhixingplan.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bsf.cqqwz.cn

[R54] 比较两个文件
来源：http://wpy.cheryme.top

diff a.txt b.txt
来源：http://cuc.hfpthk.cn

[R55] 压缩与解压
来源：http://orz.bjfxy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://apb.tanke756.top

[R56] 远程拷贝
来源：http://cmo.zhengqikj.top

scp file user@host:/path/
来源：http://cef.zdqjudy.top

[R57] 远程执行命令
来源：http://bxy.yueranfly.top

ssh user@host 'uptime'
来源：http://arb.yfazqb.com

[R58] 下载文件
来源：http://ecv.gogol.net.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lwb.jianghu66.top

[R59] 发 POST JSON
来源：http://ibh.gzhubu.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wez.ydjk.org.cn

[R60] 只看 HTTP 状态码
来源：http://dfo.jqgfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xdf.xuetiantiany.cn

[R61] 磁盘占用
来源：http://swu.xylfe.cn

df -h;  du -sh *
来源：http://eza.guannengcc.top

[R62] 找最占空间的文件
来源：http://yxl.wangdashe.top

du -ah . | sort -rh | head -10
来源：http://ulj.zhengqikj.top

[R63] 内存与进程
来源：http://kjx.yvedp.cn

free -h;  ps aux | grep nginx
来源：http://bck.fehbvm.com

[R64] 结束进程
来源：http://nig.yueranfly.top

kill -9 $(pgrep -f app.py)
来源：http://dbx.daria6918.cn

[R65] 查看端口占用
来源：http://jpr.shanyushiyangtech.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cln.cdnleiting.top

[R66] 定时任务
来源：http://vxr.sufxvd.cn

crontab -e;  crontab -l
来源：http://jwd.aibaodan.cn

[R67] 生成随机十六进制串
来源：http://bdi.hysaishi.cn

openssl rand -hex 16
来源：http://zrb.nanxuanxn.top

[R68] 计算文件校验值
来源：http://dpa.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sps.sweek.top

[R69] 生成随机密码
来源：http://cmc.daria6918.cn

head -c 16 /dev/urandom | base64
来源：http://rdd.quarkkingdee.top

[R70] 时间戳与互转
来源：http://iun.pengpengdd.cyou

date +%s;  date -d @1700000000
来源：http://dac.hesvh.cn

[R71] 日期格式化
来源：http://kxw.dashuyun.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ile.kuanghao11.cn

[R72] 等待端口就绪
来源：http://vnx.xingfuxueyuan.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://yhv.feifeiyinyue.top

[R73] 分割大日志
来源：http://mgg.zhijiandao.cn

split -l 1000 big.log part_
来源：http://utp.haohaochexian.top

[R74] 批量重命名
来源：http://axm.aibaodan.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jjj.yueranfly.top

[R75] 导出环境变量
来源：http://rlg.ivvv.top

export PATH="$HOME/bin:$PATH"
来源：http://yyq.chenzaomai.com

[R76] 使用临时文件
来源：http://qzb.jianghu66.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fms.tianlin.xyz

[R77] 读取用户输入
来源：http://mhv.jinyuanbaomall.cn

read -rp "请输入: " ans
来源：http://uhy.andypj.xyz

[R78] 交互式菜单
来源：http://xvp.wangdashe.top

select opt in a b c; do echo "$opt"; break; done
来源：http://buq.shanyushiyangtech.top

[R79] 解析命令行选项
来源：http://jao.zhixingplan.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://uvl.zhijiandao.cn

[R80] 查看脚本执行耗时
来源：http://aqo.aizwys.cn

time ./run.sh
来源：http://pyb.xylfe.cn

================================================================================
来源：http://cbq.hnxiangtu.top

S. C / C++ 专题
来源：http://mhk.redwolf501.top

================================================================================
来源：http://jas.jinqigufen.top

[S01] C：Hello World
来源：http://qkd.zhoulong.xyz

#include <stdio.h>
来源：http://eki.yj20258.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://joa.ctjpmb.com

[S02] C：变量与格式化输出
来源：http://ivc.svipenyu.cn

int a = 10; printf("%d\n", a);
来源：http://krs.sweek.top

[S03] C：读入整数
来源：http://pjq.cdnleiting.top

int x; scanf("%d", &x);
来源：http://jfx.9152youxi.cn

[S04] C：字符串复制
来源：http://mlp.fzhhl.top

char dst[32]; strcpy(dst, "hi");
来源：http://kyq.ehwqpu.com

[S05] C：字符串长度
来源：http://ymg.c1oappe.top

strlen(s)
来源：http://mqm.jqgufenzy.top

[S06] C：字符串比较
来源：http://xah.zhengqikj.top

strcmp(a, b) == 0
来源：http://muw.ctjpmb.com

[S07] C：数组遍历求和
来源：http://fyd.316326.xyz


<!-- 参考信息 -->