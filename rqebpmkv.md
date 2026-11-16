代发 wailian999

[Q44] IN 子查询
来源：http://jko.shanyushiyangkeji.top

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://drn.snrcjt.cn

[Q45] EXISTS 判断存在
来源：http://kyi.ydzc1.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://czw.xylfe.cn

[Q46] NOT EXISTS 判断不存在
来源：http://yqa.jinghuilouyu.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://dfa.fengsongda.top

[Q47] 与平均值比较
来源：http://jjl.hywenlv.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rvq.ivvv.top

[Q48] CTE 公用表表达式
来源：http://hxx.fengsongda.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://yhx.cashguo.top

SELECT * FROM t WHERE c > 5;
来源：http://skb.xinyue.icu

[Q49] 更新单行
来源：http://jak.xinyue.icu

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rme.hongshengwenyu.top

[Q50] 批量更新
来源：http://ndg.fzhhl.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vgl.316326.xyz

[Q51] 用子查询更新
来源：http://vun.aibaodan.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://afs.dashuyun.cn

[Q52] 删除指定行
来源：http://kmt.yj20258888.top

DELETE FROM users WHERE id = 10;
来源：http://dlj.zhengqikj.top

[Q53] 按条件删除
来源：http://uij.shanyushiyangkeji.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ckf.9152youxi.cn

[Q54] 清空表
来源：http://mqj.xinyue.icu

TRUNCATE TABLE logs;
来源：http://gph.xuanzx.com

[Q55] 排名（并列占位）
来源：http://fog.vqdsnc.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://epi.hongshengwenyu.top

[Q56] 密集排名（并列不占位）
来源：http://sig.shangyingyoupin.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://lsq.sysykeji.top

[Q57] 行号
来源：http://uco.tian-w.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://yug.gaohongyu789.top

[Q58] 累计求和
来源：http://wax.sxryk.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://eqg.uphjek.com

[Q59] 分组内累计
来源：http://gvj.hywenlv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://laf.yj20258888.top

[Q60] 取上一行 / 下一行
来源：http://wru.ivvv.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://srq.andypj.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zvs.yj20258.top

[Q61] 移动平均
来源：http://mda.iojbl.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hnd.smart0.xyz

[Q62] 分组占比
来源：http://yry.hnxiangtu.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://tvq.meibo888.top

[Q63] 开启事务
来源：http://ytr.zycfv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://oqi.sysykeji.top

[Q64] 提交事务
来源：http://rio.andypj.xyz

COMMIT;
来源：http://sdi.vehdjk.com

[Q65] 回滚事务
来源：http://dyh.shanyushiyangkeji.top

ROLLBACK;
来源：http://qcf.cucudq.cn

[Q66] 行锁查询
来源：http://pqx.tianlin.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rzv.daria6918.cn

[Q67] 设置隔离级别
来源：http://ass.gotoacloud.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://evu.jinqigfzy.top

[Q68] 保存点
来源：http://zpg.316326.xyz

SAVEPOINT sp1;
来源：http://nve.hongshengwenyu.top

ROLLBACK TO sp1;
来源：http://fzk.aizwys.cn

[Q69] 查看执行计划
来源：http://mok.vqdsnc.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ryy.daxiang520.top

[Q70] 更新统计信息
来源：http://lzo.quarkkingdee.top

ANALYZE TABLE users;
来源：http://lfy.jlsjyb.cn

[Q71] 查看建表语句
来源：http://els.jyoumei.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://brx.ctjpmb.com

[Q72] 查看索引
来源：http://toz.xuanzx.com

SHOW INDEX FROM users;
来源：http://dsw.xinyue.icu

[Q73] 查看表状态
来源：http://ggg.fktsv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://tor.wangdashe.top

[Q74] 强制使用索引
来源：http://eri.xylfe.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://usx.fktsv.cn

[Q75] 日期格式化
来源：http://tvq.yonumen.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://spy.hywenlv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fob.yj202588.top

[Q76] 按天统计
来源：http://cxb.hongshengwenyu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dti.jinqigufen.top

[Q77] 时间加减
来源：http://pll.dashuyun.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://woi.pengpengdd.cyou

[Q78] 当前时间
来源：http://uvs.zdbjq.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nuc.yj202588.top

[Q79] 字符串拼接
来源：http://bph.ywan-chungtsiang.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://sgx.hongshengwenyu.top

[Q80] 字符串截取
来源：http://iiq.fktsv.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zgg.vehdjk.com

[Q81] 字符串替换
来源：http://xdh.xingfuxueyuan.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dqn.shuidangran.top

[Q82] 字符长度与字节长度
来源：http://ruc.gzhubu.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://yld.tarul.cn

[Q83] 大小写转换
来源：http://qba.jinqigufen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wyb.chenlongwang.top

[Q84] 去除首尾空格
来源：http://gas.chenjidiqi.icu

SELECT TRIM(name) FROM users;
来源：http://vqk.mhx1999.top

[Q85] 数值取整
来源：http://ibh.yueranfly.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://drg.pycfn.com

[Q86] 读取 JSON 字段
来源：http://rtk.cdnleiting.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://rxx.shanyushiyangtech.top

[Q87] JSON 字段做条件
来源：http://bwj.hnxiangtu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oze.daxiang520.top

[Q88] 行转列（条件聚合）
来源：http://nvd.nwbrower.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://aav.uphjek.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://umt.ybcxt.top

[Q89] 判断表是否存在
来源：http://fin.vqdsnc.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://snq.bjfxy.top

[Q90] 生成序号列
来源：http://tdx.ctjpmb.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wqp.shangyingyoupin.top

================================================================================
来源：http://jfy.zhoulong.xyz

R. Bash 专题
来源：http://zbb.yuanzhike.top

================================================================================
来源：http://ukf.zhaomingkeji.xyz

[R01] shebang 与严格模式
来源：http://mlh.bjfxy.top

#!/usr/bin/env bash
来源：http://vxh.ydzc1.top

set -euo pipefail
来源：http://jbg.tianlin.xyz

[R02] 变量赋值与使用
来源：http://oec.nwbrower.top

name="Tom"; echo "$name"
来源：http://fvz.shanyushiyangtech.top

[R03] 只读变量
来源：http://ycq.jqgufenzy.top

readonly PI=3.14
来源：http://qjj.haohaochexian.top

[R04] 位置参数
来源：http://ccj.wangdashe.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://fww.gzhubu.top

[R05] 参数默认值
来源：http://zwg.fzhhl.top

name="${1:-default}"
来源：http://ktg.sjlbkw.cn

[R06] 判断命令是否存在
来源：http://qqw.xziqi.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://oyl.chenjidiqi.icu

[R07] if 判断文件
来源：http://olv.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cis.gogol.net.cn

[R08] 数值比较
来源：http://bdr.hnxiangtu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cyd.jlsjyb.cn

[R09] 字符串比较
来源：http://kkh.smart0.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hik.hfpthk.cn

[R10] 正则匹配
来源：http://tos.cheryme.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://uyf.ivvv.top

[R11] case 多分支
来源：http://mnu.yvedp.cn

case "$1" in
来源：http://ipm.ehwqpu.com

start) echo "启动" ;;
来源：http://npa.hongshengwenyu.top

stop)  echo "停止" ;;
来源：http://jwi.fengsongda.top

*)     echo "未知命令" ;;
来源：http://uxj.gotoacloud.top

esac
来源：http://yzr.gotoacloud.top

[R12] for 遍历文件
来源：http://dlo.zdbjq.cn

for f in *.txt; do echo "$f"; done
来源：http://udo.haohaochexian.top

[R13] for 计数循环
来源：http://itc.yj202588.top

for i in {1..10}; do echo "$i"; done
来源：http://lwu.hongshengwenyu.top

[R14] C 风格 for
来源：http://dkd.wangdashe.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wqz.yangfankeji.com

[R15] while 逐行读文件
来源：http://oxs.redwolf501.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://gaf.ydjk.org.cn

[R16] until 等待条件
来源：http://tay.yonumen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://gaj.ppjwa.cn

[R17] 数组定义与取值
来源：http://zrg.dianchejie.cn

arr=(a b c); echo "${arr[0]}"
来源：http://ewh.fengsongda.top

[R18] 遍历数组
来源：http://wri.jianghu66.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ayu.316326.xyz

[R19] 数组长度
来源：http://npq.jiagoushi.top

echo "${#arr[@]}"
来源：http://tld.aibaodan.cn

[R20] 关联数组（字典）
来源：http://xom.yonumen.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://boq.sjlbkw.cn

[R21] 字符串长度
来源：http://vhv.pycfn.com

echo "${#s}"
来源：http://tpa.tarul.cn

[R22] 截取子串
来源：http://dqp.iojbl.cn

echo "${s:0:5}"
来源：http://nya.tarul.cn

[R23] 字符串替换
来源：http://uxm.pengpengdd.cyou

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://osd.chenzaomai.com

[R24] 大小写转换
来源：http://rdb.0kj1m.cn

echo "${s^^}"; echo "${s,,}"
来源：http://pry.xinyue.icu

[R25] 去后缀 / 去前缀
来源：http://apm.tianlin.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://mre.tianlin.xyz

[R26] 命令替换
来源：http://vsy.shanyushiyangkeji.top

now=$(date +%F); echo "$now"
来源：http://tkv.gzhubu.top

[R27] 算术展开
来源：http://ljg.dianchejie.cn

echo $((1 + 2 * 3))
来源：http://wbn.meibo888.top

[R28] 浮点运算
来源：http://onv.yfazqb.com

echo "scale=2; 10/3" | bc
来源：http://xws.nanxuanxn.top

[R29] 定义函数
来源：http://ies.ehwqpu.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hxk.hcnkem.com

[R30] 函数返回状态码
来源：http://uft.havefunace.top

f() { return 0; }; f || echo "失败了"
来源：http://std.pengpengdd.cyou

[R31] 局部变量
来源：http://jkx.hnxiangtu.top

f() { local x=1; echo "$x"; }
来源：http://xmz.zhijiandao.cn

[R32] 参数个数校验
来源：http://rqc.shangyingyoupin.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gjp.ppjwa.cn

[R33] 捕获错误并提示行号
来源：http://ozt.hysaishi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dnh.jiagoushi.top

[R34] 退出时清理
来源：http://chr.9152youxi.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lzz.zhaomingkeji.xyz

[R35] 后台执行并等待
来源：http://udl.cdnleiting.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dki.chenlongwang.top

[R36] 并发执行多个任务
来源：http://eyw.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://fjh.ctjpmb.com

[R37] 把输出赋给变量
来源：http://qqk.yangfankeji.com

files=$(ls -1)
来源：http://ido.birdmap.top

[R38] 管道串联
来源：http://jxf.nanxinkj.top

cat a.txt | grep -i error | wc -l
来源：http://hwi.chenjidiqi.icu

[R39] 重定向标准输出与错误
来源：http://egh.tanke756.top

cmd > out.log 2>&1
来源：http://zhc.c1oappe.top

[R40] 追加写日志
来源：http://ahr.iojbl.cn

echo "log" >> out.log
来源：http://eeu.chenzaomai.com

[R41] 丢弃输出
来源：http://jzp.guannengcc.top

cmd >/dev/null 2>&1
来源：http://cmj.sysykeji.top

[R42] 输入重定向
来源：http://gac.yuanzhike.top

wc -l < a.txt
来源：http://mxk.sysykeji.top

[R43] 按名字查找文件
来源：http://mvf.redwolf501.top

find . -name "*.log" -type f
来源：http://fhi.yongpay.top

[R44] 按修改时间查找
来源：http://lol.vqdsnc.cn

find . -mtime -7 -type f
来源：http://bvg.hywenlv.cn

[R45] 批量删除
来源：http://guc.fzhhl.top

find . -name "*.tmp" -delete
来源：http://anc.jinqigfzy.top

[R46] 递归替换文件内容
来源：http://wip.yangfankeji.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vpq.chenjidiqi.icu

[R47] sed 单行替换
来源：http://wmt.yongpay.top

sed -i 's/foo/bar/g' a.txt
来源：http://zip.yfazqb.com

[R48] awk 取指定列
来源：http://lso.hnqzz.top

awk '{print $1, $3}' a.txt
来源：http://vwp.yangfankeji.com

[R49] awk 带条件
来源：http://jsr.fzhhl.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ljy.hongshengwenyu.top

[R50] awk 求和
来源：http://qfh.sxryk.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fgn.fanxiaobao.xyz

[R51] 排序去重取前几
来源：http://pwj.ehwqpu.com

sort a.txt | uniq -c | sort -rn | head
来源：http://kpq.uphjek.com

[R52] 统计行数
来源：http://azw.cheryme.top

wc -l a.txt
来源：http://rma.jinqigfzy.top

[R53] 查看文件头与实时尾
来源：http://fsj.xylfe.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rpy.mhx1999.top

[R54] 比较两个文件
来源：http://tzg.zycfv.cn

diff a.txt b.txt
来源：http://fco.fanxiaobao.xyz

[R55] 压缩与解压
来源：http://srk.ydzc1.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://glj.svipenyu.cn

[R56] 远程拷贝
来源：http://iru.wangshuangyany.cn

scp file user@host:/path/
来源：http://weo.tanke756.top

[R57] 远程执行命令
来源：http://pgw.316326.xyz

ssh user@host 'uptime'
来源：http://gjm.zdqjudy.top

[R58] 下载文件
来源：http://hff.nanxinkj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oio.daxiang520.top

[R59] 发 POST JSON
来源：http://tlr.316326.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mnf.andypj.xyz

[R60] 只看 HTTP 状态码
来源：http://iaz.wangdashe.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ire.fengsongda.top

[R61] 磁盘占用
来源：http://dja.vehdjk.com

df -h;  du -sh *
来源：http://ipm.dianchejie.cn

[R62] 找最占空间的文件
来源：http://nri.uphjek.com

du -ah . | sort -rh | head -10
来源：http://ljb.shanyushiyangtech.top

[R63] 内存与进程
来源：http://opq.fzhhl.top

free -h;  ps aux | grep nginx
来源：http://eav.xuanzx.com

[R64] 结束进程
来源：http://wee.ctjpmb.com

kill -9 $(pgrep -f app.py)
来源：http://row.gogol.net.cn

[R65] 查看端口占用
来源：http://voi.guannengcc.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qxj.yvedp.cn

[R66] 定时任务
来源：http://gku.ydzc1.top

crontab -e;  crontab -l
来源：http://ijq.sufxvd.cn

[R67] 生成随机十六进制串
来源：http://xla.snrcjt.cn

openssl rand -hex 16
来源：http://hew.jinqigfzy.top

[R68] 计算文件校验值
来源：http://mtd.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jnv.gzhubu.top

[R69] 生成随机密码
来源：http://mai.birdmap.top

head -c 16 /dev/urandom | base64
来源：http://igs.cheryme.top

[R70] 时间戳与互转
来源：http://mna.wangdashe.top

date +%s;  date -d @1700000000
来源：http://jra.bjfxy.top

[R71] 日期格式化
来源：http://qxr.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://yjr.hywenlv.cn

[R72] 等待端口就绪
来源：http://akx.cashguo.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ruf.haohaochexian.top

[R73] 分割大日志
来源：http://zib.jqgfzy.top

split -l 1000 big.log part_
来源：http://ydu.daria6918.cn

[R74] 批量重命名
来源：http://zrs.sjlbkw.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ymg.feifeiyinyue.top

[R75] 导出环境变量
来源：http://wwx.chenjidiqi.icu

export PATH="$HOME/bin:$PATH"
来源：http://pny.xingfuxueyuan.xyz

[R76] 使用临时文件
来源：http://ygg.aizwys.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gwo.ivvv.top

[R77] 读取用户输入
来源：http://wfi.sjlbkw.cn

read -rp "请输入: " ans
来源：http://xrh.zdbjq.cn

[R78] 交互式菜单
来源：http://jfw.tarul.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hab.gogol.net.cn

[R79] 解析命令行选项
来源：http://tij.xuanzx.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://dyg.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://tsb.cdnleiting.top

time ./run.sh
来源：http://bch.cheryme.top

================================================================================
来源：http://aww.pengpengdd.cyou

S. C / C++ 专题
来源：http://bvo.snrcjt.cn

================================================================================
来源：http://gaf.yangfankeji.com

[S01] C：Hello World
来源：http://hgy.zhijiandao.cn

#include <stdio.h>
来源：http://pmk.birdmap.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ddy.jinqigfzy.top

[S02] C：变量与格式化输出
来源：http://lqh.hongshengwenyu.top

int a = 10; printf("%d\n", a);
来源：http://nom.nanxuanxn.top

[S03] C：读入整数
来源：http://bxj.xziqi.cn

int x; scanf("%d", &x);
来源：http://hrd.zdbjq.cn

[S04] C：字符串复制
来源：http://gmb.xuetiantiany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://czl.dashuyun.cn

[S05] C：字符串长度
来源：http://uzz.cqqwz.cn

strlen(s)
来源：http://iry.guowangkeji.top

[S06] C：字符串比较
来源：http://ijo.ctjpmb.com

strcmp(a, b) == 0
来源：http://chy.mhx1999.top

[S07] C：数组遍历求和
来源：http://cpr.shzxlz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lua.havefunace.top

[S08] C：动态内存分配与释放
来源：http://muq.hammf.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wyf.bjfxy.top

[S09] C：结构体定义与初始化
来源：http://wki.yonumen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sgq.daria6918.cn

[S10] C：指针与解引用
来源：http://ggy.bbcook.cn

int *p = &a;  *p = 5;
来源：http://ima.yj202588.top

[S11] C：逐行读文件
来源：http://maa.gogol.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://pof.yuanzhike.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qgw.xingfuxueyuan.xyz

fclose(f);
来源：http://alf.yfazqb.com

[S12] C：写文件
来源：http://eqo.quarkkingdee.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://eda.yuanzhike.top

[S13] C：宏定义
来源：http://caq.hnqzz.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://thd.jianghu66.top

[S14] C：枚举
来源：http://jnc.quarkkingdee.top


<!-- 参考信息 -->