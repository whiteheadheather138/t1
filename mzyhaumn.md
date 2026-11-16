代发 wailian999

[Q44] IN 子查询
来源：http://dph.9152youxi.cn

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://zkp.hfpthk.cn

[Q45] EXISTS 判断存在
来源：http://ejn.guowangkeji.top

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://xcn.zdqjudy.top

[Q46] NOT EXISTS 判断不存在
来源：http://jtt.hnqzz.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://zot.shanyushiyangkeji.top

[Q47] 与平均值比较
来源：http://chc.tanke756.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://jzx.kuanghao11.cn

[Q48] CTE 公用表表达式
来源：http://gqk.jyoumei.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://trx.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://rwf.jqgufenzy.top

[Q49] 更新单行
来源：http://gee.ydzc1.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://aqt.yj20258888.top

[Q50] 批量更新
来源：http://twt.zhongyouzk.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://gxk.xuetiantiany.cn

[Q51] 用子查询更新
来源：http://lvt.redwolf501.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://yhf.sjlbkw.cn

[Q52] 删除指定行
来源：http://wnk.bbcook.cn

DELETE FROM users WHERE id = 10;
来源：http://gji.ehwqpu.com

[Q53] 按条件删除
来源：http://vjp.sweek.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gmz.yuanzhike.top

[Q54] 清空表
来源：http://ndl.c1oappe.top

TRUNCATE TABLE logs;
来源：http://suo.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://aor.epnwcf.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://dsg.snrcjt.cn

[Q56] 密集排名（并列不占位）
来源：http://myy.kuanghao11.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ret.fengsongda.top

[Q57] 行号
来源：http://hbk.mhx1999.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://utu.chenlongwang.top

[Q58] 累计求和
来源：http://yad.zhengqikj.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lxc.gzhubu.top

[Q59] 分组内累计
来源：http://rgl.ydjk.org.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://oex.xuanzx.com

[Q60] 取上一行 / 下一行
来源：http://drh.dashuyun.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://zos.xylfe.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ckr.andypj.xyz

[Q61] 移动平均
来源：http://fsf.ybcxt.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://gmu.jianghu66.top

[Q62] 分组占比
来源：http://yby.hysaishi.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wkl.jiagoushi.top

[Q63] 开启事务
来源：http://hjo.chenlongwang.top

START TRANSACTION;                -- 或 BEGIN
来源：http://wlr.iojbl.cn

[Q64] 提交事务
来源：http://kyr.kuanghao11.cn

COMMIT;
来源：http://idy.xingfuxueyuan.xyz

[Q65] 回滚事务
来源：http://jdw.havefunace.top

ROLLBACK;
来源：http://meo.svipenyu.cn

[Q66] 行锁查询
来源：http://hcu.zhiwuduotai.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://jvz.tianlin.xyz

[Q67] 设置隔离级别
来源：http://dor.hywenlv.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://flx.tianlin.xyz

[Q68] 保存点
来源：http://rph.vqdsnc.cn

SAVEPOINT sp1;
来源：http://rfn.shzxlz.cn

ROLLBACK TO sp1;
来源：http://nfs.yj20258888.top

[Q69] 查看执行计划
来源：http://ydc.hesvh.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qnt.gzhubu.top

[Q70] 更新统计信息
来源：http://cnn.shzxlz.cn

ANALYZE TABLE users;
来源：http://hmh.yuanzhike.top

[Q71] 查看建表语句
来源：http://fnz.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://nno.smart0.xyz

[Q72] 查看索引
来源：http://xiz.wangdashe.top

SHOW INDEX FROM users;
来源：http://nnm.shzxlz.cn

[Q73] 查看表状态
来源：http://lgj.nanxinkj.top

SHOW TABLE STATUS LIKE 'users';
来源：http://afp.shuidangran.top

[Q74] 强制使用索引
来源：http://gvm.ydjk.org.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://jpm.gzhubu.top

[Q75] 日期格式化
来源：http://cax.jqgufenzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ooh.fktsv.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://njk.zhongyouzk.top

[Q76] 按天统计
来源：http://qed.smart0.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://jne.zhongyouzk.top

[Q77] 时间加减
来源：http://qzp.aizwys.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wlo.snrcjt.cn

[Q78] 当前时间
来源：http://vxj.zhongyouzk.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://gix.yuxming.cn

[Q79] 字符串拼接
来源：http://qna.havefunace.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uue.guannengcc.top

[Q80] 字符串截取
来源：http://ntu.ybcxt.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mbv.redwolf501.top

[Q81] 字符串替换
来源：http://nkr.vqdsnc.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dmk.xuetiantiany.cn

[Q82] 字符长度与字节长度
来源：http://rby.wangdashe.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://jbn.xziqi.cn

[Q83] 大小写转换
来源：http://tqv.yonumen.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fjo.svipenyu.cn

[Q84] 去除首尾空格
来源：http://nfs.tianlin.xyz

SELECT TRIM(name) FROM users;
来源：http://yen.hnqzz.top

[Q85] 数值取整
来源：http://cmq.yj202588.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xuy.hcnkem.com

[Q86] 读取 JSON 字段
来源：http://ijv.smart0.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vro.sysykeji.top

[Q87] JSON 字段做条件
来源：http://mwb.cdnleiting.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://pzu.yangfankeji.com

[Q88] 行转列（条件聚合）
来源：http://jpc.cucudq.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://jxq.9152youxi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sml.hammf.cn

[Q89] 判断表是否存在
来源：http://icp.feifeiyinyue.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ixk.xuetiantiany.cn

[Q90] 生成序号列
来源：http://xef.fanxiaobao.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://php.jianghu66.top

================================================================================
来源：http://wwj.zdbjq.cn

R. Bash 专题
来源：http://mvq.jqgfzy.top

================================================================================
来源：http://iop.nwbrower.top

[R01] shebang 与严格模式
来源：http://otw.snrcjt.cn

#!/usr/bin/env bash
来源：http://hgg.zhijiandao.cn

set -euo pipefail
来源：http://qzc.kuanghao11.cn

[R02] 变量赋值与使用
来源：http://skn.hnxiangtu.top

name="Tom"; echo "$name"
来源：http://rpx.gzhubu.top

[R03] 只读变量
来源：http://fbs.jlsjyb.cn

readonly PI=3.14
来源：http://buu.vqdsnc.cn

[R04] 位置参数
来源：http://nsz.9152youxi.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yle.tanke756.top

[R05] 参数默认值
来源：http://qkk.jinqigufen.top

name="${1:-default}"
来源：http://spf.sxryk.cn

[R06] 判断命令是否存在
来源：http://aqn.epnwcf.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://qlt.xinyue.icu

[R07] if 判断文件
来源：http://ugm.hcnkem.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vvn.zhengqikj.top

[R08] 数值比较
来源：http://fbc.sjlbkw.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://ndb.gzhubu.top

[R09] 字符串比较
来源：http://thr.tianlin.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xiw.fengsongda.top

[R10] 正则匹配
来源：http://ljj.uphjek.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ptd.316326.xyz

[R11] case 多分支
来源：http://voo.daxiang520.top

case "$1" in
来源：http://cih.hnxiangtu.top

start) echo "启动" ;;
来源：http://xst.zhaomingkeji.xyz

stop)  echo "停止" ;;
来源：http://ama.tanke756.top

*)     echo "未知命令" ;;
来源：http://npm.hesvh.cn

esac
来源：http://jls.hysaishi.cn

[R12] for 遍历文件
来源：http://bvr.havefunace.top

for f in *.txt; do echo "$f"; done
来源：http://jkz.ivvv.top

[R13] for 计数循环
来源：http://htd.cheryme.top

for i in {1..10}; do echo "$i"; done
来源：http://dyd.xziqi.cn

[R14] C 风格 for
来源：http://req.vehdjk.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zqx.316326.xyz

[R15] while 逐行读文件
来源：http://qhb.jinghuilouyu.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://frl.cdnleiting.top

[R16] until 等待条件
来源：http://rmf.ydjk.org.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://idn.zhaomingkeji.xyz

[R17] 数组定义与取值
来源：http://ccp.yueranfly.top

arr=(a b c); echo "${arr[0]}"
来源：http://opg.xuetiantiany.cn

[R18] 遍历数组
来源：http://ltm.svipenyu.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ctp.epnwcf.com

[R19] 数组长度
来源：http://ccu.shzxlz.cn

echo "${#arr[@]}"
来源：http://ebk.dianchejie.cn

[R20] 关联数组（字典）
来源：http://ghd.xuanzx.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rqr.jqgfzy.top

[R21] 字符串长度
来源：http://jfz.tian-w.cn

echo "${#s}"
来源：http://kit.birdmap.top

[R22] 截取子串
来源：http://rma.tian-w.cn

echo "${s:0:5}"
来源：http://toe.gzhubu.top

[R23] 字符串替换
来源：http://ebk.jqgfzy.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nvh.nwbrower.top

[R24] 大小写转换
来源：http://qmu.fanxiaobao.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://icb.yj20258888.top

[R25] 去后缀 / 去前缀
来源：http://udy.zhongyouzk.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ibm.cdnleiting.top

[R26] 命令替换
来源：http://zom.hnxiangtu.top

now=$(date +%F); echo "$now"
来源：http://fcw.xylfe.cn

[R27] 算术展开
来源：http://kkm.wangshuangyany.cn

echo $((1 + 2 * 3))
来源：http://jmw.sweek.top

[R28] 浮点运算
来源：http://ued.svipenyu.cn

echo "scale=2; 10/3" | bc
来源：http://smh.kuanghao11.cn

[R29] 定义函数
来源：http://uzp.hongshengwenyu.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://erz.uphjek.com

[R30] 函数返回状态码
来源：http://hnc.aizwys.cn

f() { return 0; }; f || echo "失败了"
来源：http://fkb.cashguo.top

[R31] 局部变量
来源：http://mjp.guannengcc.top

f() { local x=1; echo "$x"; }
来源：http://gms.nanxinkj.top

[R32] 参数个数校验
来源：http://aez.svipenyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mpa.hnxiangtu.top

[R33] 捕获错误并提示行号
来源：http://erl.sysykeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://xph.jqgfzy.top

[R34] 退出时清理
来源：http://gdl.fzhhl.top

trap 'rm -f "$tmp"' EXIT
来源：http://sqa.hcnkem.com

[R35] 后台执行并等待
来源：http://cgr.shangyingyoupin.top

sleep 5 & pid=$!; wait "$pid"
来源：http://iby.nwbrower.top

[R36] 并发执行多个任务
来源：http://fbz.gogol.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nip.sxryk.cn

[R37] 把输出赋给变量
来源：http://sey.yueranfly.top

files=$(ls -1)
来源：http://jgn.sxryk.cn

[R38] 管道串联
来源：http://cni.sysykeji.top

cat a.txt | grep -i error | wc -l
来源：http://pbd.sxryk.cn

[R39] 重定向标准输出与错误
来源：http://fox.sysykeji.top

cmd > out.log 2>&1
来源：http://rrh.jqgfzy.top

[R40] 追加写日志
来源：http://clo.bjfxy.top

echo "log" >> out.log
来源：http://kfy.aizwys.cn

[R41] 丢弃输出
来源：http://thd.zdbjq.cn

cmd >/dev/null 2>&1
来源：http://pep.cheryme.top

[R42] 输入重定向
来源：http://xyt.nanxuanxn.top

wc -l < a.txt
来源：http://okc.xuetiantiany.cn

[R43] 按名字查找文件
来源：http://elt.kuanghao11.cn

find . -name "*.log" -type f
来源：http://wtq.xuetiantiany.cn

[R44] 按修改时间查找
来源：http://pao.fktsv.cn

find . -mtime -7 -type f
来源：http://ask.yvedp.cn

[R45] 批量删除
来源：http://qpo.daria6918.cn

find . -name "*.tmp" -delete
来源：http://cmu.pycfn.com

[R46] 递归替换文件内容
来源：http://lyd.yonumen.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jha.fehbvm.com

[R47] sed 单行替换
来源：http://zbt.xylfe.cn

sed -i 's/foo/bar/g' a.txt
来源：http://doc.ctjpmb.com

[R48] awk 取指定列
来源：http://oqu.hnqzz.top

awk '{print $1, $3}' a.txt
来源：http://jsn.tanke756.top

[R49] awk 带条件
来源：http://kvy.yueranfly.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eno.zhaomingkeji.xyz

[R50] awk 求和
来源：http://lws.jiagoushi.top

awk '{s += $2} END {print s}' a.txt
来源：http://uua.hnxiangtu.top

[R51] 排序去重取前几
来源：http://viz.havefunace.top

sort a.txt | uniq -c | sort -rn | head
来源：http://wlv.yueranfly.top

[R52] 统计行数
来源：http://soe.andypj.xyz

wc -l a.txt
来源：http://fva.guannengcc.top

[R53] 查看文件头与实时尾
来源：http://qls.daria6918.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rzm.jqgfzy.top

[R54] 比较两个文件
来源：http://zpb.jinghuilouyu.cn

diff a.txt b.txt
来源：http://krs.ydzc1.top

[R55] 压缩与解压
来源：http://skx.yueranfly.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bjs.zdqjudy.top

[R56] 远程拷贝
来源：http://uaa.gotoacloud.top

scp file user@host:/path/
来源：http://asx.bbcook.cn

[R57] 远程执行命令
来源：http://tlu.kuanghao11.cn

ssh user@host 'uptime'
来源：http://lkm.jqgufenzy.top

[R58] 下载文件
来源：http://axd.haohaochexian.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://enn.hcnkem.com

[R59] 发 POST JSON
来源：http://ppp.meibo888.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://emu.fehbvm.com

[R60] 只看 HTTP 状态码
来源：http://ulr.shanyushiyangtech.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bsx.wangdashe.top

[R61] 磁盘占用
来源：http://wud.daria6918.cn

df -h;  du -sh *
来源：http://apk.ydzc1.top

[R62] 找最占空间的文件
来源：http://srn.redwolf501.top

du -ah . | sort -rh | head -10
来源：http://yyh.sjlbkw.cn

[R63] 内存与进程
来源：http://nay.chenlongwang.top

free -h;  ps aux | grep nginx
来源：http://xid.ydzc1.top

[R64] 结束进程
来源：http://hee.ehwqpu.com

kill -9 $(pgrep -f app.py)
来源：http://vvc.shanyushiyangkeji.top

[R65] 查看端口占用
来源：http://lpm.yuanzhike.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cei.hammf.cn

[R66] 定时任务
来源：http://xju.bjfxy.top

crontab -e;  crontab -l
来源：http://hnm.fzhhl.top

[R67] 生成随机十六进制串
来源：http://wnw.birdmap.top

openssl rand -hex 16
来源：http://csj.hfpthk.cn

[R68] 计算文件校验值
来源：http://tnm.cashguo.top

sha256sum a.txt;  md5sum a.txt
来源：http://fmx.xingfuxueyuan.xyz

[R69] 生成随机密码
来源：http://ohg.yuxming.cn

head -c 16 /dev/urandom | base64
来源：http://phm.cdnleiting.top

[R70] 时间戳与互转
来源：http://mqo.jqgfzy.top

date +%s;  date -d @1700000000
来源：http://nzc.chenzaomai.com

[R71] 日期格式化
来源：http://vdb.ehwqpu.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://cmn.iojbl.cn

[R72] 等待端口就绪
来源：http://ugt.gaohongyu789.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mjn.vehdjk.com

[R73] 分割大日志
来源：http://plm.daria6918.cn

split -l 1000 big.log part_
来源：http://kzx.yvedp.cn

[R74] 批量重命名
来源：http://mpc.xingfuxueyuan.xyz

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dhs.haohaochexian.top

[R75] 导出环境变量
来源：http://gah.9152youxi.cn

export PATH="$HOME/bin:$PATH"
来源：http://huh.chenlongwang.top

[R76] 使用临时文件
来源：http://aui.ywan-chungtsiang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hkm.cqqwz.cn

[R77] 读取用户输入
来源：http://gcg.cucudq.cn

read -rp "请输入: " ans
来源：http://zre.fanxiaobao.xyz

[R78] 交互式菜单
来源：http://bui.kuanghao11.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gxf.shanyushiyangtech.top

[R79] 解析命令行选项
来源：http://rha.zdqjudy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yke.hnxiangtu.top

[R80] 查看脚本执行耗时
来源：http://aah.ydjk.org.cn

time ./run.sh
来源：http://kvh.nanxuanxn.top

================================================================================
来源：http://uuj.xziqi.cn

S. C / C++ 专题
来源：http://mbs.gotoacloud.top

================================================================================
来源：http://qfo.yuxming.cn

[S01] C：Hello World
来源：http://gks.yvedp.cn

#include <stdio.h>
来源：http://ujy.wangdashe.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://fex.cqqwz.cn

[S02] C：变量与格式化输出
来源：http://jrl.redwolf501.top

int a = 10; printf("%d\n", a);
来源：http://dye.pycfn.com

[S03] C：读入整数
来源：http://rgx.cashguo.top

int x; scanf("%d", &x);
来源：http://xkn.jinqigfzy.top

[S04] C：字符串复制
来源：http://vgp.xuetiantiany.cn

char dst[32]; strcpy(dst, "hi");
来源：http://veg.pycfn.com

[S05] C：字符串长度
来源：http://bgy.wangdashe.top

strlen(s)
来源：http://gao.hcnkem.com

[S06] C：字符串比较
来源：http://ssh.redwolf501.top

strcmp(a, b) == 0
来源：http://sox.birdmap.top

[S07] C：数组遍历求和
来源：http://gpj.guannengcc.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wjf.hnqzz.top

[S08] C：动态内存分配与释放
来源：http://nhx.haohaochexian.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vjz.xziqi.cn

[S09] C：结构体定义与初始化
来源：http://uml.316326.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cvb.shanyushiyangkeji.top

[S10] C：指针与解引用
来源：http://rlm.yfazqb.com

int *p = &a;  *p = 5;
来源：http://bfr.kuanghao11.cn

[S11] C：逐行读文件
来源：http://pcy.aizwys.cn

FILE *f = fopen("a.txt", "r");
来源：http://klw.ppjwa.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uvl.jinqigfzy.top

fclose(f);
来源：http://kgj.ppjwa.cn

[S12] C：写文件
来源：http://bsa.jinqigufen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jdp.yuxming.cn

[S13] C：宏定义
来源：http://kyn.0kj1m.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rtm.birdmap.top

[S14] C：枚举
来源：http://msv.jinqigfzy.top


<!-- 参考信息 -->