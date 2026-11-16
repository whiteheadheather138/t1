代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://xxq.cheryme.top

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://fvs.iojbl.cn

[Q47] 与平均值比较
来源：http://qmu.snrcjt.cn

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wfu.vehdjk.com

[Q48] CTE 公用表表达式
来源：http://pmh.snrcjt.cn

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://lnc.sjlbkw.cn

SELECT * FROM t WHERE c > 5;
来源：http://utn.guannengcc.top

[Q49] 更新单行
来源：http://xtf.ehwqpu.com

UPDATE users SET status = 1 WHERE id = 10;
来源：http://txs.jinghuilouyu.cn

[Q50] 批量更新
来源：http://iom.uphjek.com

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ftu.yanxiufei.cn

[Q51] 用子查询更新
来源：http://zuk.jianghu66.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hxu.zycfv.cn

[Q52] 删除指定行
来源：http://vdh.9152youxi.cn

DELETE FROM users WHERE id = 10;
来源：http://dpe.ydjk.org.cn

[Q53] 按条件删除
来源：http://ala.yj20258888.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fge.ehwqpu.com

[Q54] 清空表
来源：http://iha.mhx1999.top

TRUNCATE TABLE logs;
来源：http://twb.zhongyouzk.top

[Q55] 排名（并列占位）
来源：http://fwp.fzhhl.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sqs.fktsv.cn

[Q56] 密集排名（并列不占位）
来源：http://wkt.daria6918.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://odf.haohaochexian.top

[Q57] 行号
来源：http://olc.tianlin.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://zch.bbcook.cn

[Q58] 累计求和
来源：http://fxu.ppjwa.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://urz.tian-w.cn

[Q59] 分组内累计
来源：http://qtd.0kj1m.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://zhm.zdbjq.cn

[Q60] 取上一行 / 下一行
来源：http://nfz.yuxming.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://qvg.cashguo.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dmb.jinqigfzy.top

[Q61] 移动平均
来源：http://ddb.haohaochexian.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aae.jinqigfzy.top

[Q62] 分组占比
来源：http://qgf.cdnleiting.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://jwq.chenzaomai.com

[Q63] 开启事务
来源：http://yfb.redwolf501.top

START TRANSACTION;                -- 或 BEGIN
来源：http://hwv.jinyuanbaomall.cn

[Q64] 提交事务
来源：http://yld.fanxiaobao.xyz

COMMIT;
来源：http://tso.dianchejie.cn

[Q65] 回滚事务
来源：http://aev.hongshengwenyu.top

ROLLBACK;
来源：http://pts.svipenyu.cn

[Q66] 行锁查询
来源：http://ofx.yanxiufei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qjz.yanxiufei.cn

[Q67] 设置隔离级别
来源：http://shf.guowangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zyh.ppjwa.cn

[Q68] 保存点
来源：http://qrg.xuetiantiany.cn

SAVEPOINT sp1;
来源：http://btb.zhengqikj.top

ROLLBACK TO sp1;
来源：http://gmb.bbcook.cn

[Q69] 查看执行计划
来源：http://pcw.xziqi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://kwh.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://jnc.fzhhl.top

ANALYZE TABLE users;
来源：http://zhd.fanxiaobao.xyz

[Q71] 查看建表语句
来源：http://zjm.jinghuilouyu.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wkp.jqgufenzy.top

[Q72] 查看索引
来源：http://oip.yueranfly.top

SHOW INDEX FROM users;
来源：http://ijq.zhaomingkeji.xyz

[Q73] 查看表状态
来源：http://ipf.ivvv.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qbr.jyoumei.cn

[Q74] 强制使用索引
来源：http://jgy.gzhubu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://dkx.pengpengdd.cyou

[Q75] 日期格式化
来源：http://iku.chenzaomai.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://sqt.c1oappe.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qet.nwbrower.top

[Q76] 按天统计
来源：http://zqs.zhixingplan.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ywl.zhiwuduotai.top

[Q77] 时间加减
来源：http://cfi.hammf.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://brn.daria6918.cn

[Q78] 当前时间
来源：http://qfw.yanxiufei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ryq.yanxiufei.cn

[Q79] 字符串拼接
来源：http://hvu.gaohongyu789.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qki.cdnleiting.top

[Q80] 字符串截取
来源：http://vus.havefunace.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://szd.nwbrower.top

[Q81] 字符串替换
来源：http://ass.ehwqpu.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tso.yueranfly.top

[Q82] 字符长度与字节长度
来源：http://pbj.kuanghao11.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ern.andypj.xyz

[Q83] 大小写转换
来源：http://gwm.jinqigfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ysw.jiagoushi.top

[Q84] 去除首尾空格
来源：http://qxw.ppjwa.cn

SELECT TRIM(name) FROM users;
来源：http://skt.bbcook.cn

[Q85] 数值取整
来源：http://sns.quarkkingdee.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mai.gzhubu.top

[Q86] 读取 JSON 字段
来源：http://ofh.shuidangran.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xbc.chenjidiqi.icu

[Q87] JSON 字段做条件
来源：http://wqi.chenzaomai.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://gkw.vqdsnc.cn

[Q88] 行转列（条件聚合）
来源：http://njo.ydzc1.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://eys.hesvh.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rta.smart0.xyz

[Q89] 判断表是否存在
来源：http://asm.jianghu66.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nyx.yonumen.top

[Q90] 生成序号列
来源：http://jiz.hysaishi.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ksb.pengpengdd.cyou

================================================================================
来源：http://xqd.hongshengwenyu.top

R. Bash 专题
来源：http://dia.hnqzz.top

================================================================================
来源：http://lwr.zdqjudy.top

[R01] shebang 与严格模式
来源：http://sqd.sxryk.cn

#!/usr/bin/env bash
来源：http://ldl.ehwqpu.com

set -euo pipefail
来源：http://cmv.xuetiantiany.cn

[R02] 变量赋值与使用
来源：http://kbw.hesvh.cn

name="Tom"; echo "$name"
来源：http://bid.epnwcf.com

[R03] 只读变量
来源：http://sns.hfpthk.cn

readonly PI=3.14
来源：http://slc.uphjek.com

[R04] 位置参数
来源：http://nda.shanyushiyangtech.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://lev.yfazqb.com

[R05] 参数默认值
来源：http://aby.sysykeji.top

name="${1:-default}"
来源：http://qhh.zhaomingkeji.xyz

[R06] 判断命令是否存在
来源：http://yqk.hammf.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://lrw.dianchejie.cn

[R07] if 判断文件
来源：http://gcj.yanxiufei.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://dxm.chenlongwang.top

[R08] 数值比较
来源：http://vje.havefunace.top

if (( a > b )); then echo "a 更大"; fi
来源：http://erw.guowangkeji.top

[R09] 字符串比较
来源：http://uin.zdqjudy.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kua.sufxvd.cn

[R10] 正则匹配
来源：http://hui.hnxiangtu.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://czn.jlsjyb.cn

[R11] case 多分支
来源：http://iga.52xcode.cn

case "$1" in
来源：http://bea.bjfxy.top

start) echo "启动" ;;
来源：http://tda.fengsongda.top

stop)  echo "停止" ;;
来源：http://snm.redwolf501.top

*)     echo "未知命令" ;;
来源：http://pma.zycfv.cn

esac
来源：http://vfh.zhengqikj.top

[R12] for 遍历文件
来源：http://olm.nanxuanxn.top

for f in *.txt; do echo "$f"; done
来源：http://vkc.zhixingplan.top

[R13] for 计数循环
来源：http://ysm.fengsongda.top

for i in {1..10}; do echo "$i"; done
来源：http://bzn.yj20258.top

[R14] C 风格 for
来源：http://teg.hammf.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tzv.xuetiantiany.cn

[R15] while 逐行读文件
来源：http://zri.ydzc1.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oci.fanxiaobao.xyz

[R16] until 等待条件
来源：http://itf.nwbrower.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://txi.cheryme.top

[R17] 数组定义与取值
来源：http://prj.guowangkeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://wce.yj20258.top

[R18] 遍历数组
来源：http://hwj.yangfankeji.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ary.ppjwa.cn

[R19] 数组长度
来源：http://gut.gotoacloud.top

echo "${#arr[@]}"
来源：http://nsq.gogol.net.cn

[R20] 关联数组（字典）
来源：http://egz.ydjk.org.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jsh.guannengcc.top

[R21] 字符串长度
来源：http://roj.pengpengdd.cyou

echo "${#s}"
来源：http://yug.jinqigufen.top

[R22] 截取子串
来源：http://bas.zhijiandao.cn

echo "${s:0:5}"
来源：http://bkm.svipenyu.cn

[R23] 字符串替换
来源：http://jdn.tian-w.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://bit.zhijiandao.cn

[R24] 大小写转换
来源：http://mye.vehdjk.com

echo "${s^^}"; echo "${s,,}"
来源：http://asw.tian-w.cn

[R25] 去后缀 / 去前缀
来源：http://gvg.shzxlz.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://gbr.vqdsnc.cn

[R26] 命令替换
来源：http://yzu.c1oappe.top

now=$(date +%F); echo "$now"
来源：http://oba.yfazqb.com

[R27] 算术展开
来源：http://cwx.snrcjt.cn

echo $((1 + 2 * 3))
来源：http://bhe.nanxinkj.top

[R28] 浮点运算
来源：http://prm.tianlin.xyz

echo "scale=2; 10/3" | bc
来源：http://ehj.yueranfly.top

[R29] 定义函数
来源：http://yib.haohaochexian.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ccc.nwbrower.top

[R30] 函数返回状态码
来源：http://vfo.hongshengwenyu.top

f() { return 0; }; f || echo "失败了"
来源：http://jpe.hnxiangtu.top

[R31] 局部变量
来源：http://ahe.andypj.xyz

f() { local x=1; echo "$x"; }
来源：http://qje.zhijiandao.cn

[R32] 参数个数校验
来源：http://dwt.sysykeji.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hgx.zhaomingkeji.xyz

[R33] 捕获错误并提示行号
来源：http://lhe.aizwys.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://gbp.snrcjt.cn

[R34] 退出时清理
来源：http://jpf.redwolf501.top

trap 'rm -f "$tmp"' EXIT
来源：http://rov.dashuyun.cn

[R35] 后台执行并等待
来源：http://gkw.hywenlv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://klq.aibaodan.cn

[R36] 并发执行多个任务
来源：http://rel.zhongyouzk.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mzb.dianchejie.cn

[R37] 把输出赋给变量
来源：http://iow.fzhhl.top

files=$(ls -1)
来源：http://kye.pengpengdd.cyou

[R38] 管道串联
来源：http://ptp.smart0.xyz

cat a.txt | grep -i error | wc -l
来源：http://gqw.gzhubu.top

[R39] 重定向标准输出与错误
来源：http://hjo.redwolf501.top

cmd > out.log 2>&1
来源：http://sqq.aibaodan.cn

[R40] 追加写日志
来源：http://fur.uphjek.com

echo "log" >> out.log
来源：http://yga.jiagoushi.top

[R41] 丢弃输出
来源：http://vai.gogol.net.cn

cmd >/dev/null 2>&1
来源：http://asb.pycfn.com

[R42] 输入重定向
来源：http://mlr.aizwys.cn

wc -l < a.txt
来源：http://eqg.hysaishi.cn

[R43] 按名字查找文件
来源：http://prp.c1oappe.top

find . -name "*.log" -type f
来源：http://ccw.zdqjudy.top

[R44] 按修改时间查找
来源：http://roa.jlsjyb.cn

find . -mtime -7 -type f
来源：http://jjx.havefunace.top

[R45] 批量删除
来源：http://wiy.guowangkeji.top

find . -name "*.tmp" -delete
来源：http://fjs.zhijiandao.cn

[R46] 递归替换文件内容
来源：http://upq.0kj1m.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hxc.yj202588.top

[R47] sed 单行替换
来源：http://ylk.hfpthk.cn

sed -i 's/foo/bar/g' a.txt
来源：http://nri.haohaochexian.top

[R48] awk 取指定列
来源：http://chg.jyoumei.cn

awk '{print $1, $3}' a.txt
来源：http://bje.xuanzx.com

[R49] awk 带条件
来源：http://jee.sjlbkw.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nas.vehdjk.com

[R50] awk 求和
来源：http://ojo.aibaodan.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ifv.aizwys.cn

[R51] 排序去重取前几
来源：http://wcx.smart0.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://gck.jinghuilouyu.cn

[R52] 统计行数
来源：http://pie.cqqwz.cn

wc -l a.txt
来源：http://sno.gogol.net.cn

[R53] 查看文件头与实时尾
来源：http://anv.redwolf501.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ijk.guowangkeji.top

[R54] 比较两个文件
来源：http://wxv.nanxuanxn.top

diff a.txt b.txt
来源：http://axh.hcnkem.com

[R55] 压缩与解压
来源：http://ecs.ctjpmb.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://omb.fanxiaobao.xyz

[R56] 远程拷贝
来源：http://wgw.snrcjt.cn

scp file user@host:/path/
来源：http://eip.bjfxy.top

[R57] 远程执行命令
来源：http://ucx.gogol.net.cn

ssh user@host 'uptime'
来源：http://qst.yonumen.top

[R58] 下载文件
来源：http://tyr.ywan-chungtsiang.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xxv.dianchejie.cn

[R59] 发 POST JSON
来源：http://ezl.kuanghao11.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zcs.hesvh.cn

[R60] 只看 HTTP 状态码
来源：http://ael.sweek.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wvf.sysykeji.top

[R61] 磁盘占用
来源：http://hsd.cdnleiting.top

df -h;  du -sh *
来源：http://rap.chenzaomai.com

[R62] 找最占空间的文件
来源：http://lnk.zhongyouzk.top

du -ah . | sort -rh | head -10
来源：http://vkg.hnxiangtu.top

[R63] 内存与进程
来源：http://fpr.nanxinkj.top

free -h;  ps aux | grep nginx
来源：http://itd.iojbl.cn

[R64] 结束进程
来源：http://boj.jinyuanbaomall.cn

kill -9 $(pgrep -f app.py)
来源：http://uau.zhoulong.xyz

[R65] 查看端口占用
来源：http://ppu.gogol.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://phy.gzhubu.top

[R66] 定时任务
来源：http://zvk.zhaomingkeji.xyz

crontab -e;  crontab -l
来源：http://est.havefunace.top

[R67] 生成随机十六进制串
来源：http://rls.fanxiaobao.xyz

openssl rand -hex 16
来源：http://qto.hcnkem.com

[R68] 计算文件校验值
来源：http://ger.kuanghao11.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ylg.shangyingyoupin.top

[R69] 生成随机密码
来源：http://man.nanxinkj.top

head -c 16 /dev/urandom | base64
来源：http://jeg.daxiang520.top

[R70] 时间戳与互转
来源：http://axt.fzhhl.top

date +%s;  date -d @1700000000
来源：http://gju.guowangkeji.top

[R71] 日期格式化
来源：http://ruf.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://mau.xingfuxueyuan.xyz

[R72] 等待端口就绪
来源：http://shi.yangfankeji.com

until nc -z localhost 3306; do sleep 1; done
来源：http://sdn.wangshuangyany.cn

[R73] 分割大日志
来源：http://nky.hnqzz.top

split -l 1000 big.log part_
来源：http://abq.ctjpmb.com

[R74] 批量重命名
来源：http://ros.xziqi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ulg.hywenlv.cn

[R75] 导出环境变量
来源：http://lph.wangshuangyany.cn

export PATH="$HOME/bin:$PATH"
来源：http://nnu.meibo888.top

[R76] 使用临时文件
来源：http://lua.dianchejie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ptb.xuetiantiany.cn

[R77] 读取用户输入
来源：http://kvn.yueranfly.top

read -rp "请输入: " ans
来源：http://atb.dashuyun.cn

[R78] 交互式菜单
来源：http://tzf.jiagoushi.top

select opt in a b c; do echo "$opt"; break; done
来源：http://qua.xingfuxueyuan.xyz

[R79] 解析命令行选项
来源：http://zyl.9152youxi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bcg.jinghuilouyu.cn

[R80] 查看脚本执行耗时
来源：http://scn.bjfxy.top

time ./run.sh
来源：http://tpy.yonumen.top

================================================================================
来源：http://tzn.epnwcf.com

S. C / C++ 专题
来源：http://jku.haohaochexian.top

================================================================================
来源：http://wkl.jiagoushi.top

[S01] C：Hello World
来源：http://loc.gotoacloud.top

#include <stdio.h>
来源：http://uwh.zhiwuduotai.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://htd.zdqjudy.top

[S02] C：变量与格式化输出
来源：http://hjf.ivvv.top

int a = 10; printf("%d\n", a);
来源：http://qbs.yueranfly.top

[S03] C：读入整数
来源：http://zty.kuanghao11.cn

int x; scanf("%d", &x);
来源：http://rex.fehbvm.com

[S04] C：字符串复制
来源：http://dsf.xinyue.icu

char dst[32]; strcpy(dst, "hi");
来源：http://kws.chenzaomai.com

[S05] C：字符串长度
来源：http://wuu.epnwcf.com

strlen(s)
来源：http://pdv.jianghu66.top

[S06] C：字符串比较
来源：http://kpe.daxiang520.top

strcmp(a, b) == 0
来源：http://xpr.zhaomingkeji.xyz

[S07] C：数组遍历求和
来源：http://mce.hywenlv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mtq.fehbvm.com

[S08] C：动态内存分配与释放
来源：http://mgk.wangshuangyany.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ahd.ppjwa.cn

[S09] C：结构体定义与初始化
来源：http://fhy.yuanzhike.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qam.wangdashe.top

[S10] C：指针与解引用
来源：http://puk.kuanghao11.cn

int *p = &a;  *p = 5;
来源：http://fgw.hesvh.cn

[S11] C：逐行读文件
来源：http://pvk.ctjpmb.com

FILE *f = fopen("a.txt", "r");
来源：http://hpe.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tmx.sxryk.cn

fclose(f);
来源：http://yxb.ydjk.org.cn

[S12] C：写文件
来源：http://ebp.jinqigufen.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bpz.bbcook.cn

[S13] C：宏定义
来源：http://dds.tarul.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jcr.tianlin.xyz

[S14] C：枚举
来源：http://nga.0kj1m.cn

enum Color { RED, GREEN, BLUE };
来源：http://pwt.pycfn.com

[S15] C：类型转换
来源：http://jnf.gogol.net.cn

(double) a / b
来源：http://fpl.chenlongwang.top

[S16] C：位操作置位
来源：http://ovz.cheryme.top


<!-- 参考信息 -->