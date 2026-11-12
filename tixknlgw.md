代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://ikw.0kj1m.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wgh.yj20258.top

[Q47] 与平均值比较
来源：http://scj.cheryme.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://dlb.havefunace.top

[Q48] CTE 公用表表达式
来源：http://zjn.zhengqikj.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://dlt.chenlongwang.top

SELECT * FROM t WHERE c > 5;
来源：http://ycq.haohaochexian.top

[Q49] 更新单行
来源：http://ihw.xziqi.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://vbf.cdnleiting.top

[Q50] 批量更新
来源：http://pmp.bbcook.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://ulh.yj20258888.top

[Q51] 用子查询更新
来源：http://ija.hesvh.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://smy.svipenyu.cn

[Q52] 删除指定行
来源：http://iky.gzhubu.top

DELETE FROM users WHERE id = 10;
来源：http://kjz.xuanzx.com

[Q53] 按条件删除
来源：http://xgr.cqqwz.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://cbk.jiagoushi.top

[Q54] 清空表
来源：http://pzb.jinqigufen.top

TRUNCATE TABLE logs;
来源：http://qge.chenjidiqi.icu

[Q55] 排名（并列占位）
来源：http://was.yuanzhike.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mmv.sufxvd.cn

[Q56] 密集排名（并列不占位）
来源：http://ufx.fzhhl.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://yur.yuanzhike.top

[Q57] 行号
来源：http://trh.zdbjq.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://sxp.jiagoushi.top

[Q58] 累计求和
来源：http://trd.jyoumei.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://biq.jiagoushi.top

[Q59] 分组内累计
来源：http://kvl.iojbl.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://nko.svipenyu.cn

[Q60] 取上一行 / 下一行
来源：http://mus.pycfn.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://dzo.yangfankeji.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ebl.9152youxi.cn

[Q61] 移动平均
来源：http://uab.andypj.xyz

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pxy.zhongyouzk.top

[Q62] 分组占比
来源：http://dro.yj20258888.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://lnu.ybcxt.top

[Q63] 开启事务
来源：http://kge.kuanghao11.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://ion.yanxiufei.cn

[Q64] 提交事务
来源：http://ujj.shanyushiyangkeji.top

COMMIT;
来源：http://hes.tanke756.top

[Q65] 回滚事务
来源：http://kbb.uphjek.com

ROLLBACK;
来源：http://aea.xuanzx.com

[Q66] 行锁查询
来源：http://tqo.ybcxt.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bvh.cdnleiting.top

[Q67] 设置隔离级别
来源：http://enn.shanyushiyangtech.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rrp.aizwys.cn

[Q68] 保存点
来源：http://zfl.hcnkem.com

SAVEPOINT sp1;
来源：http://mst.chenlongwang.top

ROLLBACK TO sp1;
来源：http://sra.redwolf501.top

[Q69] 查看执行计划
来源：http://sft.jiagoushi.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://oba.birdmap.top

[Q70] 更新统计信息
来源：http://cmu.zhaomingkeji.xyz

ANALYZE TABLE users;
来源：http://phg.zhaomingkeji.xyz

[Q71] 查看建表语句
来源：http://eon.zhoulong.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://tyy.yj20258888.top

[Q72] 查看索引
来源：http://myn.zycfv.cn

SHOW INDEX FROM users;
来源：http://pgz.zhiwuduotai.top

[Q73] 查看表状态
来源：http://grk.tian-w.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://mzd.hywenlv.cn

[Q74] 强制使用索引
来源：http://nwi.wangshuangyany.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://qww.fanxiaobao.xyz

[Q75] 日期格式化
来源：http://zjt.yj20258.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://scj.jiagoushi.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kob.nanxinkj.top

[Q76] 按天统计
来源：http://aze.jqgfzy.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fwb.cucudq.cn

[Q77] 时间加减
来源：http://agw.cdnleiting.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://tep.pengpengdd.cyou

[Q78] 当前时间
来源：http://bbc.snrcjt.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://sbf.yfazqb.com

[Q79] 字符串拼接
来源：http://gvt.hnqzz.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tjz.c1oappe.top

[Q80] 字符串截取
来源：http://svq.yuanzhike.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yky.dashuyun.cn

[Q81] 字符串替换
来源：http://zyf.smart0.xyz

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ybd.cqqwz.cn

[Q82] 字符长度与字节长度
来源：http://ezj.haohaochexian.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zzs.gaohongyu789.top

[Q83] 大小写转换
来源：http://mje.ehwqpu.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://whj.ctjpmb.com

[Q84] 去除首尾空格
来源：http://dbg.shzxlz.cn

SELECT TRIM(name) FROM users;
来源：http://qjw.zhixingplan.top

[Q85] 数值取整
来源：http://uvw.ctjpmb.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://cvf.kuanghao11.cn

[Q86] 读取 JSON 字段
来源：http://pkd.chenjidiqi.icu

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://jvi.ywan-chungtsiang.top

[Q87] JSON 字段做条件
来源：http://dhc.yueranfly.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://glo.wangshuangyany.cn

[Q88] 行转列（条件聚合）
来源：http://emw.shzxlz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://gng.hysaishi.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://rfi.hcnkem.com

[Q89] 判断表是否存在
来源：http://idj.haohaochexian.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cjp.fktsv.cn

[Q90] 生成序号列
来源：http://gdu.jianghu66.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tbg.aizwys.cn

================================================================================
来源：http://oxb.sweek.top

R. Bash 专题
来源：http://gml.shangyingyoupin.top

================================================================================
来源：http://bna.tanke756.top

[R01] shebang 与严格模式
来源：http://pax.gotoacloud.top

#!/usr/bin/env bash
来源：http://nnw.jqgufenzy.top

set -euo pipefail
来源：http://qzk.chenjidiqi.icu

[R02] 变量赋值与使用
来源：http://wyt.hywenlv.cn

name="Tom"; echo "$name"
来源：http://svm.bbcook.cn

[R03] 只读变量
来源：http://xws.mhx1999.top

readonly PI=3.14
来源：http://dvw.316326.xyz

[R04] 位置参数
来源：http://vxa.hongshengwenyu.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jzc.ydzc1.top

[R05] 参数默认值
来源：http://cmu.hcnkem.com

name="${1:-default}"
来源：http://pxb.hammf.cn

[R06] 判断命令是否存在
来源：http://zed.shzxlz.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://whb.jianghu66.top

[R07] if 判断文件
来源：http://fkh.sysykeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jdi.gogol.net.cn

[R08] 数值比较
来源：http://pmb.yuanzhike.top

if (( a > b )); then echo "a 更大"; fi
来源：http://sxp.daria6918.cn

[R09] 字符串比较
来源：http://pms.xuanzx.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bhx.pycfn.com

[R10] 正则匹配
来源：http://wcz.havefunace.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://fio.aibaodan.cn

[R11] case 多分支
来源：http://ygc.ywan-chungtsiang.top

case "$1" in
来源：http://eca.guowangkeji.top

start) echo "启动" ;;
来源：http://imd.52xcode.cn

stop)  echo "停止" ;;
来源：http://ftt.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://ktj.jianghu66.top

esac
来源：http://jgx.hammf.cn

[R12] for 遍历文件
来源：http://avc.hnqzz.top

for f in *.txt; do echo "$f"; done
来源：http://tsu.chenlongwang.top

[R13] for 计数循环
来源：http://kwr.yangfankeji.com

for i in {1..10}; do echo "$i"; done
来源：http://kyv.yfazqb.com

[R14] C 风格 for
来源：http://vug.hnxiangtu.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://sum.hesvh.cn

[R15] while 逐行读文件
来源：http://mcl.316326.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pfo.yj20258888.top

[R16] until 等待条件
来源：http://agx.yanxiufei.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://kty.cqqwz.cn

[R17] 数组定义与取值
来源：http://wkx.kuanghao11.cn

arr=(a b c); echo "${arr[0]}"
来源：http://csh.feifeiyinyue.top

[R18] 遍历数组
来源：http://bpx.ivvv.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sph.sysykeji.top

[R19] 数组长度
来源：http://dxs.guannengcc.top

echo "${#arr[@]}"
来源：http://ivy.redwolf501.top

[R20] 关联数组（字典）
来源：http://xdf.hesvh.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hos.xingfuxueyuan.xyz

[R21] 字符串长度
来源：http://ntb.yvedp.cn

echo "${#s}"
来源：http://ose.zhengqikj.top

[R22] 截取子串
来源：http://nhd.nwbrower.top

echo "${s:0:5}"
来源：http://iur.xingfuxueyuan.xyz

[R23] 字符串替换
来源：http://atf.jinghuilouyu.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mvg.cucudq.cn

[R24] 大小写转换
来源：http://csi.ydjk.org.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nmd.havefunace.top

[R25] 去后缀 / 去前缀
来源：http://jkz.hongshengwenyu.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ftp.jinqigufen.top

[R26] 命令替换
来源：http://hnb.ydjk.org.cn

now=$(date +%F); echo "$now"
来源：http://vjm.316326.xyz

[R27] 算术展开
来源：http://pzj.jinqigufen.top

echo $((1 + 2 * 3))
来源：http://npf.zhixingplan.top

[R28] 浮点运算
来源：http://tws.shzxlz.cn

echo "scale=2; 10/3" | bc
来源：http://jvl.fehbvm.com

[R29] 定义函数
来源：http://aom.tanke756.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xdn.hywenlv.cn

[R30] 函数返回状态码
来源：http://tea.hywenlv.cn

f() { return 0; }; f || echo "失败了"
来源：http://zep.316326.xyz

[R31] 局部变量
来源：http://yyk.redwolf501.top

f() { local x=1; echo "$x"; }
来源：http://ujj.ywan-chungtsiang.top

[R32] 参数个数校验
来源：http://pwj.quarkkingdee.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mko.zhengqikj.top

[R33] 捕获错误并提示行号
来源：http://pbk.hywenlv.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bxg.sweek.top

[R34] 退出时清理
来源：http://yaj.chenlongwang.top

trap 'rm -f "$tmp"' EXIT
来源：http://nzs.ppjwa.cn

[R35] 后台执行并等待
来源：http://lcc.jinqigfzy.top

sleep 5 & pid=$!; wait "$pid"
来源：http://nsl.shanyushiyangtech.top

[R36] 并发执行多个任务
来源：http://jzm.hongshengwenyu.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ujh.shuidangran.top

[R37] 把输出赋给变量
来源：http://mgl.hysaishi.cn

files=$(ls -1)
来源：http://yig.nwbrower.top

[R38] 管道串联
来源：http://ked.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://fkr.xuetiantiany.cn

[R39] 重定向标准输出与错误
来源：http://zhc.daria6918.cn

cmd > out.log 2>&1
来源：http://naw.jinyuanbaomall.cn

[R40] 追加写日志
来源：http://mcv.ehwqpu.com

echo "log" >> out.log
来源：http://rgq.yuxming.cn

[R41] 丢弃输出
来源：http://bjg.tarul.cn

cmd >/dev/null 2>&1
来源：http://rsg.zhixingplan.top

[R42] 输入重定向
来源：http://aya.hnqzz.top

wc -l < a.txt
来源：http://pko.daria6918.cn

[R43] 按名字查找文件
来源：http://pdm.bbcook.cn

find . -name "*.log" -type f
来源：http://lvr.hnxiangtu.top

[R44] 按修改时间查找
来源：http://lbz.yj20258888.top

find . -mtime -7 -type f
来源：http://jae.yuanzhike.top

[R45] 批量删除
来源：http://vlo.pycfn.com

find . -name "*.tmp" -delete
来源：http://hyu.feifeiyinyue.top

[R46] 递归替换文件内容
来源：http://jkg.redwolf501.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://vov.yuxming.cn

[R47] sed 单行替换
来源：http://fdd.ywan-chungtsiang.top

sed -i 's/foo/bar/g' a.txt
来源：http://mwp.jiagoushi.top

[R48] awk 取指定列
来源：http://uqk.pycfn.com

awk '{print $1, $3}' a.txt
来源：http://gee.gotoacloud.top

[R49] awk 带条件
来源：http://usq.havefunace.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gct.epnwcf.com

[R50] awk 求和
来源：http://ouf.vqdsnc.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nos.bjfxy.top

[R51] 排序去重取前几
来源：http://ybg.tarul.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://kgb.zhixingplan.top

[R52] 统计行数
来源：http://ila.havefunace.top

wc -l a.txt
来源：http://jqd.cheryme.top

[R53] 查看文件头与实时尾
来源：http://dat.xingfuxueyuan.xyz

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jnf.aizwys.cn

[R54] 比较两个文件
来源：http://qwi.yonumen.top

diff a.txt b.txt
来源：http://acv.zhiwuduotai.top

[R55] 压缩与解压
来源：http://teb.hammf.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xxt.haohaochexian.top

[R56] 远程拷贝
来源：http://orb.quarkkingdee.top

scp file user@host:/path/
来源：http://zbt.jyoumei.cn

[R57] 远程执行命令
来源：http://zfl.hysaishi.cn

ssh user@host 'uptime'
来源：http://tei.wangshuangyany.cn

[R58] 下载文件
来源：http://usw.shangyingyoupin.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vhe.bjfxy.top

[R59] 发 POST JSON
来源：http://dxz.quarkkingdee.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jgj.nanxuanxn.top

[R60] 只看 HTTP 状态码
来源：http://qxy.vehdjk.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cqf.jinghuilouyu.cn

[R61] 磁盘占用
来源：http://ywk.jqgufenzy.top

df -h;  du -sh *
来源：http://wzb.zycfv.cn

[R62] 找最占空间的文件
来源：http://gwu.snrcjt.cn

du -ah . | sort -rh | head -10
来源：http://faj.0kj1m.cn

[R63] 内存与进程
来源：http://fjx.xziqi.cn

free -h;  ps aux | grep nginx
来源：http://lcn.shuidangran.top

[R64] 结束进程
来源：http://ufd.dianchejie.cn

kill -9 $(pgrep -f app.py)
来源：http://fkp.xziqi.cn

[R65] 查看端口占用
来源：http://lpi.chenlongwang.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yuk.sjlbkw.cn

[R66] 定时任务
来源：http://sug.zdqjudy.top

crontab -e;  crontab -l
来源：http://iji.xziqi.cn

[R67] 生成随机十六进制串
来源：http://rvp.uphjek.com

openssl rand -hex 16
来源：http://ewa.hongshengwenyu.top

[R68] 计算文件校验值
来源：http://aip.redwolf501.top

sha256sum a.txt;  md5sum a.txt
来源：http://chj.zhijiandao.cn

[R69] 生成随机密码
来源：http://xyp.nwbrower.top

head -c 16 /dev/urandom | base64
来源：http://rbz.hysaishi.cn

[R70] 时间戳与互转
来源：http://qmh.tarul.cn

date +%s;  date -d @1700000000
来源：http://xva.aibaodan.cn

[R71] 日期格式化
来源：http://oxb.dashuyun.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yzv.hysaishi.cn

[R72] 等待端口就绪
来源：http://zbi.wangshuangyany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xlu.shuidangran.top

[R73] 分割大日志
来源：http://uyl.gogol.net.cn

split -l 1000 big.log part_
来源：http://uni.316326.xyz

[R74] 批量重命名
来源：http://xhm.yfazqb.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oja.daxiang520.top

[R75] 导出环境变量
来源：http://dqs.c1oappe.top

export PATH="$HOME/bin:$PATH"
来源：http://fxm.mhx1999.top

[R76] 使用临时文件
来源：http://iea.yj202588.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://vil.dashuyun.cn

[R77] 读取用户输入
来源：http://wcc.shanyushiyangkeji.top

read -rp "请输入: " ans
来源：http://pbw.yuanzhike.top

[R78] 交互式菜单
来源：http://efi.tianlin.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://iso.aibaodan.cn

[R79] 解析命令行选项
来源：http://sah.shanyushiyangkeji.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nnv.vqdsnc.cn

[R80] 查看脚本执行耗时
来源：http://hlz.cashguo.top

time ./run.sh
来源：http://kmc.meibo888.top

================================================================================
来源：http://vix.yj20258888.top

S. C / C++ 专题
来源：http://dbh.ywan-chungtsiang.top

================================================================================
来源：http://bop.yonumen.top

[S01] C：Hello World
来源：http://dgt.c1oappe.top

#include <stdio.h>
来源：http://mpq.chenjidiqi.icu

int main(void) { printf("Hello\n"); return 0; }
来源：http://hsp.shanyushiyangtech.top

[S02] C：变量与格式化输出
来源：http://kbp.sjlbkw.cn

int a = 10; printf("%d\n", a);
来源：http://vvu.tarul.cn

[S03] C：读入整数
来源：http://alz.jlsjyb.cn

int x; scanf("%d", &x);
来源：http://hah.gotoacloud.top

[S04] C：字符串复制
来源：http://dhz.gotoacloud.top

char dst[32]; strcpy(dst, "hi");
来源：http://nst.gzhubu.top

[S05] C：字符串长度
来源：http://izv.hcnkem.com

strlen(s)
来源：http://teu.jqgufenzy.top

[S06] C：字符串比较
来源：http://yzz.aibaodan.cn

strcmp(a, b) == 0
来源：http://eou.hesvh.cn

[S07] C：数组遍历求和
来源：http://fyf.hysaishi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ijf.chenjidiqi.icu

[S08] C：动态内存分配与释放
来源：http://iqi.redwolf501.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://afk.0kj1m.cn

[S09] C：结构体定义与初始化
来源：http://oar.fehbvm.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gpb.mhx1999.top

[S10] C：指针与解引用
来源：http://gjk.quarkkingdee.top

int *p = &a;  *p = 5;
来源：http://xea.sjlbkw.cn

[S11] C：逐行读文件
来源：http://pgn.havefunace.top

FILE *f = fopen("a.txt", "r");
来源：http://psy.vqdsnc.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://qqg.xziqi.cn

fclose(f);
来源：http://wqk.hnqzz.top

[S12] C：写文件
来源：http://uaq.dashuyun.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fns.hongshengwenyu.top

[S13] C：宏定义
来源：http://bpj.zhoulong.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://raf.dianchejie.cn

[S14] C：枚举
来源：http://hlr.chenlongwang.top

enum Color { RED, GREEN, BLUE };
来源：http://vbh.ctjpmb.com

[S15] C：类型转换
来源：http://jvi.zhiwuduotai.top

(double) a / b
来源：http://doq.aizwys.cn

[S16] C：位操作置位
来源：http://rvj.jianghu66.top


<!-- 参考信息 -->