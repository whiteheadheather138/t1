代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://ifp.yvedp.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wfz.fehbvm.com

[Q47] 与平均值比较
来源：http://ord.hongshengwenyu.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://rep.tian-w.cn

[Q48] CTE 公用表表达式
来源：http://etp.chenlongwang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://ncr.jqgfzy.top

SELECT * FROM t WHERE c > 5;
来源：http://zmy.shanyushiyangkeji.top

[Q49] 更新单行
来源：http://lif.hammf.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://rbv.yuxming.cn

[Q50] 批量更新
来源：http://twy.yvedp.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mse.hywenlv.cn

[Q51] 用子查询更新
来源：http://axi.jlsjyb.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://xon.jianghu66.top

[Q52] 删除指定行
来源：http://brh.yueranfly.top

DELETE FROM users WHERE id = 10;
来源：http://wyt.jinqigfzy.top

[Q53] 按条件删除
来源：http://rhb.ppjwa.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ybp.shanyushiyangkeji.top

[Q54] 清空表
来源：http://wvl.pengpengdd.cyou

TRUNCATE TABLE logs;
来源：http://enw.jyoumei.cn

[Q55] 排名（并列占位）
来源：http://mcn.hywenlv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wtf.dashuyun.cn

[Q56] 密集排名（并列不占位）
来源：http://bts.aizwys.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mcz.svipenyu.cn

[Q57] 行号
来源：http://sax.dianchejie.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://gei.shanyushiyangtech.top

[Q58] 累计求和
来源：http://wjw.aizwys.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://nie.yfazqb.com

[Q59] 分组内累计
来源：http://zsv.aizwys.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://kjv.xinyue.icu

[Q60] 取上一行 / 下一行
来源：http://dhl.birdmap.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://jhs.iojbl.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hgm.sjlbkw.cn

[Q61] 移动平均
来源：http://saz.yfazqb.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://edm.ppjwa.cn

[Q62] 分组占比
来源：http://zgv.epnwcf.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ipj.feifeiyinyue.top

[Q63] 开启事务
来源：http://ncc.uphjek.com

START TRANSACTION;                -- 或 BEGIN
来源：http://kfe.bjfxy.top

[Q64] 提交事务
来源：http://yup.kuanghao11.cn

COMMIT;
来源：http://syj.zycfv.cn

[Q65] 回滚事务
来源：http://niy.gzhubu.top

ROLLBACK;
来源：http://fpn.kuanghao11.cn

[Q66] 行锁查询
来源：http://yww.tarul.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nsg.quarkkingdee.top

[Q67] 设置隔离级别
来源：http://dgm.xuetiantiany.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://bml.9152youxi.cn

[Q68] 保存点
来源：http://yde.dianchejie.cn

SAVEPOINT sp1;
来源：http://pic.cashguo.top

ROLLBACK TO sp1;
来源：http://lwr.hesvh.cn

[Q69] 查看执行计划
来源：http://akt.havefunace.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ijd.vehdjk.com

[Q70] 更新统计信息
来源：http://mrf.smart0.xyz

ANALYZE TABLE users;
来源：http://ypz.ydjk.org.cn

[Q71] 查看建表语句
来源：http://wlp.sufxvd.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wdy.zdqjudy.top

[Q72] 查看索引
来源：http://mgd.dashuyun.cn

SHOW INDEX FROM users;
来源：http://sfd.sufxvd.cn

[Q73] 查看表状态
来源：http://nsr.hywenlv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://zrn.svipenyu.cn

[Q74] 强制使用索引
来源：http://nhw.xziqi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://iro.zhijiandao.cn

[Q75] 日期格式化
来源：http://yyz.meibo888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://kiq.yanxiufei.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://btr.wangdashe.top

[Q76] 按天统计
来源：http://qih.hongshengwenyu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://elo.ydzc1.top

[Q77] 时间加减
来源：http://bdc.yangfankeji.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vxh.ybcxt.top

[Q78] 当前时间
来源：http://aii.tian-w.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nxu.fengsongda.top

[Q79] 字符串拼接
来源：http://xqg.vqdsnc.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zsm.quarkkingdee.top

[Q80] 字符串截取
来源：http://tle.jinghuilouyu.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gwm.ydjk.org.cn

[Q81] 字符串替换
来源：http://xiy.cheryme.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://iai.tanke756.top

[Q82] 字符长度与字节长度
来源：http://erw.xuetiantiany.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://tbg.xingfuxueyuan.xyz

[Q83] 大小写转换
来源：http://bbn.redwolf501.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wlr.pycfn.com

[Q84] 去除首尾空格
来源：http://qhq.9152youxi.cn

SELECT TRIM(name) FROM users;
来源：http://wuo.wangdashe.top

[Q85] 数值取整
来源：http://zgx.bjfxy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qwz.snrcjt.cn

[Q86] 读取 JSON 字段
来源：http://afk.shanyushiyangtech.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ugv.daria6918.cn

[Q87] JSON 字段做条件
来源：http://oxd.yongpay.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://int.fanxiaobao.xyz

[Q88] 行转列（条件聚合）
来源：http://dcd.cdnleiting.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://pkl.tarul.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pci.tarul.cn

[Q89] 判断表是否存在
来源：http://nyr.xuanzx.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fok.zdqjudy.top

[Q90] 生成序号列
来源：http://rjm.haohaochexian.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sne.cashguo.top

================================================================================
来源：http://hep.zdbjq.cn

R. Bash 专题
来源：http://zoy.xuetiantiany.cn

================================================================================
来源：http://yhr.52xcode.cn

[R01] shebang 与严格模式
来源：http://hdj.tarul.cn

#!/usr/bin/env bash
来源：http://xst.fktsv.cn

set -euo pipefail
来源：http://ojr.birdmap.top

[R02] 变量赋值与使用
来源：http://vnj.yangfankeji.com

name="Tom"; echo "$name"
来源：http://opl.yuxming.cn

[R03] 只读变量
来源：http://ffg.hesvh.cn

readonly PI=3.14
来源：http://jpz.feifeiyinyue.top

[R04] 位置参数
来源：http://hgp.nwbrower.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ueq.mhx1999.top

[R05] 参数默认值
来源：http://tbz.aibaodan.cn

name="${1:-default}"
来源：http://lct.zhongyouzk.top

[R06] 判断命令是否存在
来源：http://xfn.cucudq.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sah.sxryk.cn

[R07] if 判断文件
来源：http://muu.jinyuanbaomall.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://pvf.ehwqpu.com

[R08] 数值比较
来源：http://qsv.yuxming.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://lpn.guowangkeji.top

[R09] 字符串比较
来源：http://jea.wangshuangyany.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://cze.sjlbkw.cn

[R10] 正则匹配
来源：http://oni.quarkkingdee.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nlr.hesvh.cn

[R11] case 多分支
来源：http://bhr.hnqzz.top

case "$1" in
来源：http://tpe.fengsongda.top

start) echo "启动" ;;
来源：http://nns.jiagoushi.top

stop)  echo "停止" ;;
来源：http://rpa.jinyuanbaomall.cn

*)     echo "未知命令" ;;
来源：http://avm.jinyuanbaomall.cn

esac
来源：http://jbo.zhoulong.xyz

[R12] for 遍历文件
来源：http://dfr.svipenyu.cn

for f in *.txt; do echo "$f"; done
来源：http://lqz.zycfv.cn

[R13] for 计数循环
来源：http://otf.chenlongwang.top

for i in {1..10}; do echo "$i"; done
来源：http://ekx.hammf.cn

[R14] C 风格 for
来源：http://sxr.yvedp.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vlp.xinyue.icu

[R15] while 逐行读文件
来源：http://jbp.hnqzz.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://aur.52xcode.cn

[R16] until 等待条件
来源：http://mwf.jiagoushi.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://iyx.bjfxy.top

[R17] 数组定义与取值
来源：http://tgi.yj202588.top

arr=(a b c); echo "${arr[0]}"
来源：http://gjm.nanxinkj.top

[R18] 遍历数组
来源：http://vtq.chenlongwang.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ivr.gzhubu.top

[R19] 数组长度
来源：http://txt.nanxinkj.top

echo "${#arr[@]}"
来源：http://lqk.ctjpmb.com

[R20] 关联数组（字典）
来源：http://okx.gzhubu.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://aub.cucudq.cn

[R21] 字符串长度
来源：http://otz.wangshuangyany.cn

echo "${#s}"
来源：http://lsx.jqgufenzy.top

[R22] 截取子串
来源：http://pcj.yj20258888.top

echo "${s:0:5}"
来源：http://rtg.gotoacloud.top

[R23] 字符串替换
来源：http://yhh.yongpay.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hqh.ywan-chungtsiang.top

[R24] 大小写转换
来源：http://pgj.sjlbkw.cn

echo "${s^^}"; echo "${s,,}"
来源：http://iok.cucudq.cn

[R25] 去后缀 / 去前缀
来源：http://gqc.mhx1999.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://cby.xylfe.cn

[R26] 命令替换
来源：http://giy.shzxlz.cn

now=$(date +%F); echo "$now"
来源：http://mhh.vqdsnc.cn

[R27] 算术展开
来源：http://caj.vehdjk.com

echo $((1 + 2 * 3))
来源：http://jaj.ivvv.top

[R28] 浮点运算
来源：http://kzk.tarul.cn

echo "scale=2; 10/3" | bc
来源：http://smv.fktsv.cn

[R29] 定义函数
来源：http://wmg.jqgfzy.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://coj.gogol.net.cn

[R30] 函数返回状态码
来源：http://pko.sufxvd.cn

f() { return 0; }; f || echo "失败了"
来源：http://ajr.hongshengwenyu.top

[R31] 局部变量
来源：http://eoj.svipenyu.cn

f() { local x=1; echo "$x"; }
来源：http://wsg.ydjk.org.cn

[R32] 参数个数校验
来源：http://tmg.daxiang520.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fqp.chenlongwang.top

[R33] 捕获错误并提示行号
来源：http://lrc.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ach.nanxinkj.top

[R34] 退出时清理
来源：http://ksf.hongshengwenyu.top

trap 'rm -f "$tmp"' EXIT
来源：http://tis.nanxinkj.top

[R35] 后台执行并等待
来源：http://cmt.andypj.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://xai.jinyuanbaomall.cn

[R36] 并发执行多个任务
来源：http://kui.cashguo.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xpe.tian-w.cn

[R37] 把输出赋给变量
来源：http://die.tarul.cn

files=$(ls -1)
来源：http://wfd.jinghuilouyu.cn

[R38] 管道串联
来源：http://emz.shanyushiyangtech.top

cat a.txt | grep -i error | wc -l
来源：http://loj.gaohongyu789.top

[R39] 重定向标准输出与错误
来源：http://mjm.xylfe.cn

cmd > out.log 2>&1
来源：http://gce.gaohongyu789.top

[R40] 追加写日志
来源：http://lzz.zhongyouzk.top

echo "log" >> out.log
来源：http://pgf.chenzaomai.com

[R41] 丢弃输出
来源：http://rwy.wangshuangyany.cn

cmd >/dev/null 2>&1
来源：http://yha.tarul.cn

[R42] 输入重定向
来源：http://wel.redwolf501.top

wc -l < a.txt
来源：http://amu.yj202588.top

[R43] 按名字查找文件
来源：http://nde.hnqzz.top

find . -name "*.log" -type f
来源：http://qjz.tian-w.cn

[R44] 按修改时间查找
来源：http://fdu.daria6918.cn

find . -mtime -7 -type f
来源：http://qmw.wangdashe.top

[R45] 批量删除
来源：http://wcr.zhixingplan.top

find . -name "*.tmp" -delete
来源：http://zmx.hesvh.cn

[R46] 递归替换文件内容
来源：http://gat.nanxinkj.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://cae.xuetiantiany.cn

[R47] sed 单行替换
来源：http://azr.sysykeji.top

sed -i 's/foo/bar/g' a.txt
来源：http://gnv.yfazqb.com

[R48] awk 取指定列
来源：http://bqz.hfpthk.cn

awk '{print $1, $3}' a.txt
来源：http://isd.hammf.cn

[R49] awk 带条件
来源：http://upe.ctjpmb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xhv.cqqwz.cn

[R50] awk 求和
来源：http://zgc.wangshuangyany.cn

awk '{s += $2} END {print s}' a.txt
来源：http://gva.xinyue.icu

[R51] 排序去重取前几
来源：http://epe.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vgs.xinyue.icu

[R52] 统计行数
来源：http://vbp.haohaochexian.top

wc -l a.txt
来源：http://ujl.yanxiufei.cn

[R53] 查看文件头与实时尾
来源：http://klf.fengsongda.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://vwz.gaohongyu789.top

[R54] 比较两个文件
来源：http://lzo.jlsjyb.cn

diff a.txt b.txt
来源：http://ili.yj202588.top

[R55] 压缩与解压
来源：http://tfq.yj20258.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nnv.bbcook.cn

[R56] 远程拷贝
来源：http://kcz.birdmap.top

scp file user@host:/path/
来源：http://jjs.jinqigfzy.top

[R57] 远程执行命令
来源：http://vmf.ehwqpu.com

ssh user@host 'uptime'
来源：http://jzb.fehbvm.com

[R58] 下载文件
来源：http://mhp.yj20258.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nrm.jiagoushi.top

[R59] 发 POST JSON
来源：http://ofy.chenjidiqi.icu

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://skg.vehdjk.com

[R60] 只看 HTTP 状态码
来源：http://keo.fehbvm.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zwu.chenlongwang.top

[R61] 磁盘占用
来源：http://bed.fengsongda.top

df -h;  du -sh *
来源：http://ytc.gotoacloud.top

[R62] 找最占空间的文件
来源：http://cgc.pycfn.com

du -ah . | sort -rh | head -10
来源：http://mmb.sweek.top

[R63] 内存与进程
来源：http://suu.yj202588.top

free -h;  ps aux | grep nginx
来源：http://lth.xuanzx.com

[R64] 结束进程
来源：http://pju.gogol.net.cn

kill -9 $(pgrep -f app.py)
来源：http://znf.cdnleiting.top

[R65] 查看端口占用
来源：http://tlr.jinyuanbaomall.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://iqr.jiagoushi.top

[R66] 定时任务
来源：http://oql.xuanzx.com

crontab -e;  crontab -l
来源：http://awy.redwolf501.top

[R67] 生成随机十六进制串
来源：http://lre.sjlbkw.cn

openssl rand -hex 16
来源：http://mdn.ehwqpu.com

[R68] 计算文件校验值
来源：http://ldz.mhx1999.top

sha256sum a.txt;  md5sum a.txt
来源：http://ety.sjlbkw.cn

[R69] 生成随机密码
来源：http://bwu.yj20258.top

head -c 16 /dev/urandom | base64
来源：http://pcl.yuanzhike.top

[R70] 时间戳与互转
来源：http://zdy.xylfe.cn

date +%s;  date -d @1700000000
来源：http://hlx.wangshuangyany.cn

[R71] 日期格式化
来源：http://bbt.cdnleiting.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://clm.316326.xyz

[R72] 等待端口就绪
来源：http://exh.fzhhl.top

until nc -z localhost 3306; do sleep 1; done
来源：http://mmx.sysykeji.top

[R73] 分割大日志
来源：http://oma.9152youxi.cn

split -l 1000 big.log part_
来源：http://aqo.ywan-chungtsiang.top

[R74] 批量重命名
来源：http://efl.zdbjq.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://web.yuanzhike.top

[R75] 导出环境变量
来源：http://nsb.nanxinkj.top

export PATH="$HOME/bin:$PATH"
来源：http://ctf.jinqigfzy.top

[R76] 使用临时文件
来源：http://fsz.bbcook.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://oej.pengpengdd.cyou

[R77] 读取用户输入
来源：http://cox.pengpengdd.cyou

read -rp "请输入: " ans
来源：http://otp.daxiang520.top

[R78] 交互式菜单
来源：http://sdb.ctjpmb.com

select opt in a b c; do echo "$opt"; break; done
来源：http://fsz.tian-w.cn

[R79] 解析命令行选项
来源：http://prd.gaohongyu789.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vdc.andypj.xyz

[R80] 查看脚本执行耗时
来源：http://qpl.sjlbkw.cn

time ./run.sh
来源：http://njo.jqgufenzy.top

================================================================================
来源：http://jfn.daria6918.cn

S. C / C++ 专题
来源：http://vle.cdnleiting.top

================================================================================
来源：http://utj.ehwqpu.com

[S01] C：Hello World
来源：http://gdk.316326.xyz

#include <stdio.h>
来源：http://myw.jqgfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://nxt.aizwys.cn

[S02] C：变量与格式化输出
来源：http://ifi.shuidangran.top

int a = 10; printf("%d\n", a);
来源：http://uqy.fktsv.cn

[S03] C：读入整数
来源：http://aqk.jlsjyb.cn

int x; scanf("%d", &x);
来源：http://vru.quarkkingdee.top

[S04] C：字符串复制
来源：http://gwt.zycfv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cgg.wangshuangyany.cn

[S05] C：字符串长度
来源：http://fsy.zhaomingkeji.xyz

strlen(s)
来源：http://rlj.dashuyun.cn

[S06] C：字符串比较
来源：http://agl.gogol.net.cn

strcmp(a, b) == 0
来源：http://vti.nanxuanxn.top

[S07] C：数组遍历求和
来源：http://uey.fanxiaobao.xyz

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qti.chenjidiqi.icu

[S08] C：动态内存分配与释放
来源：http://vbx.tian-w.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gde.yanxiufei.cn

[S09] C：结构体定义与初始化
来源：http://pzq.tanke756.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://aam.jianghu66.top

[S10] C：指针与解引用
来源：http://qxm.aibaodan.cn

int *p = &a;  *p = 5;
来源：http://mip.zhongyouzk.top

[S11] C：逐行读文件
来源：http://hdo.yanxiufei.cn

FILE *f = fopen("a.txt", "r");
来源：http://twa.jqgufenzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pix.epnwcf.com

fclose(f);
来源：http://vrn.jinghuilouyu.cn

[S12] C：写文件
来源：http://vug.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cxa.yj20258888.top

[S13] C：宏定义
来源：http://xxv.tanke756.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dnb.sxryk.cn

[S14] C：枚举
来源：http://uco.shzxlz.cn

enum Color { RED, GREEN, BLUE };
来源：http://edm.vehdjk.com

[S15] C：类型转换
来源：http://gcl.smart0.xyz

(double) a / b
来源：http://hpp.yuanzhike.top

[S16] C：位操作置位
来源：http://zkd.zhengqikj.top


<!-- 参考信息 -->