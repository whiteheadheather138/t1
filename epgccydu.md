代发 wailian999

[Q46] NOT EXISTS 判断不存在
来源：http://xrd.52xcode.cn

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://lcj.ydjk.org.cn

[Q47] 与平均值比较
来源：http://mea.havefunace.top

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wop.jiagoushi.top

[Q48] CTE 公用表表达式
来源：http://zqn.shangyingyoupin.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xfz.gzhubu.top

SELECT * FROM t WHERE c > 5;
来源：http://ptl.yj202588.top

[Q49] 更新单行
来源：http://cbf.yongpay.top

UPDATE users SET status = 1 WHERE id = 10;
来源：http://jms.hnxiangtu.top

[Q50] 批量更新
来源：http://yob.ydzc1.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://vcv.smart0.xyz

[Q51] 用子查询更新
来源：http://jmw.haohaochexian.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rqo.mhx1999.top

[Q52] 删除指定行
来源：http://alj.cqqwz.cn

DELETE FROM users WHERE id = 10;
来源：http://hea.gogol.net.cn

[Q53] 按条件删除
来源：http://nni.gaohongyu789.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://lqw.epnwcf.com

[Q54] 清空表
来源：http://jti.yangfankeji.com

TRUNCATE TABLE logs;
来源：http://rvl.tanke756.top

[Q55] 排名（并列占位）
来源：http://zfs.bbcook.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jbw.0kj1m.cn

[Q56] 密集排名（并列不占位）
来源：http://jtq.shanyushiyangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://oco.chenzaomai.com

[Q57] 行号
来源：http://vlo.zhijiandao.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://uui.aizwys.cn

[Q58] 累计求和
来源：http://xdi.gaohongyu789.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://jlr.vehdjk.com

[Q59] 分组内累计
来源：http://ewq.cdnleiting.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ufy.chenjidiqi.icu

[Q60] 取上一行 / 下一行
来源：http://rqk.quarkkingdee.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ltr.ybcxt.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://svl.birdmap.top

[Q61] 移动平均
来源：http://kjb.nanxuanxn.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cfv.daxiang520.top

[Q62] 分组占比
来源：http://fqz.0kj1m.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yjv.ctjpmb.com

[Q63] 开启事务
来源：http://cda.zhengqikj.top

START TRANSACTION;                -- 或 BEGIN
来源：http://age.ydzc1.top

[Q64] 提交事务
来源：http://tkp.yongpay.top

COMMIT;
来源：http://uwj.jqgufenzy.top

[Q65] 回滚事务
来源：http://grg.zhongyouzk.top

ROLLBACK;
来源：http://aql.xingfuxueyuan.xyz

[Q66] 行锁查询
来源：http://mlo.iojbl.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cxq.tian-w.cn

[Q67] 设置隔离级别
来源：http://tup.tianlin.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rdy.ehwqpu.com

[Q68] 保存点
来源：http://yki.zhongyouzk.top

SAVEPOINT sp1;
来源：http://lui.bjfxy.top

ROLLBACK TO sp1;
来源：http://rje.yuxming.cn

[Q69] 查看执行计划
来源：http://eud.yfazqb.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zpr.vehdjk.com

[Q70] 更新统计信息
来源：http://bbq.quarkkingdee.top

ANALYZE TABLE users;
来源：http://uar.xinyue.icu

[Q71] 查看建表语句
来源：http://cft.yangfankeji.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ssy.tanke756.top

[Q72] 查看索引
来源：http://rpa.zhengqikj.top

SHOW INDEX FROM users;
来源：http://xqx.ivvv.top

[Q73] 查看表状态
来源：http://wld.ydzc1.top

SHOW TABLE STATUS LIKE 'users';
来源：http://blo.cashguo.top

[Q74] 强制使用索引
来源：http://xtl.fengsongda.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rhh.zhongyouzk.top

[Q75] 日期格式化
来源：http://uoj.yj20258888.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fxm.daria6918.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fvj.ivvv.top

[Q76] 按天统计
来源：http://gqr.snrcjt.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://idz.jinqigfzy.top

[Q77] 时间加减
来源：http://zvb.shanyushiyangtech.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hqb.xuetiantiany.cn

[Q78] 当前时间
来源：http://cod.redwolf501.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qst.aizwys.cn

[Q79] 字符串拼接
来源：http://wch.daxiang520.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://jde.hammf.cn

[Q80] 字符串截取
来源：http://bll.meibo888.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://pmc.jinqigfzy.top

[Q81] 字符串替换
来源：http://lwi.yanxiufei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://tfx.tianlin.xyz

[Q82] 字符长度与字节长度
来源：http://lly.chenjidiqi.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uiq.ywan-chungtsiang.top

[Q83] 大小写转换
来源：http://tep.fengsongda.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://iuo.ctjpmb.com

[Q84] 去除首尾空格
来源：http://hew.shanyushiyangkeji.top

SELECT TRIM(name) FROM users;
来源：http://chy.ywan-chungtsiang.top

[Q85] 数值取整
来源：http://aol.tian-w.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nlr.haohaochexian.top

[Q86] 读取 JSON 字段
来源：http://wmg.c1oappe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://okz.yanxiufei.cn

[Q87] JSON 字段做条件
来源：http://zdh.52xcode.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fak.ydjk.org.cn

[Q88] 行转列（条件聚合）
来源：http://yeg.snrcjt.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://tcn.wangshuangyany.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://snr.shangyingyoupin.top

[Q89] 判断表是否存在
来源：http://ogm.jianghu66.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wqw.daxiang520.top

[Q90] 生成序号列
来源：http://agx.gaohongyu789.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ytl.zhongyouzk.top

================================================================================
来源：http://jbn.cashguo.top

R. Bash 专题
来源：http://iit.haohaochexian.top

================================================================================
来源：http://hlb.nanxuanxn.top

[R01] shebang 与严格模式
来源：http://epo.quarkkingdee.top

#!/usr/bin/env bash
来源：http://ehr.gogol.net.cn

set -euo pipefail
来源：http://bot.tian-w.cn

[R02] 变量赋值与使用
来源：http://gft.jinyuanbaomall.cn

name="Tom"; echo "$name"
来源：http://hpk.feifeiyinyue.top

[R03] 只读变量
来源：http://ihl.ppjwa.cn

readonly PI=3.14
来源：http://uia.9152youxi.cn

[R04] 位置参数
来源：http://mhv.sweek.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://pxr.ppjwa.cn

[R05] 参数默认值
来源：http://mxq.feifeiyinyue.top

name="${1:-default}"
来源：http://bgx.tarul.cn

[R06] 判断命令是否存在
来源：http://wne.guannengcc.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tac.vqdsnc.cn

[R07] if 判断文件
来源：http://mfj.shuidangran.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://eza.redwolf501.top

[R08] 数值比较
来源：http://eri.chenjidiqi.icu

if (( a > b )); then echo "a 更大"; fi
来源：http://epx.zdbjq.cn

[R09] 字符串比较
来源：http://gic.zhoulong.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kym.mhx1999.top

[R10] 正则匹配
来源：http://bwv.xziqi.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wqc.gotoacloud.top

[R11] case 多分支
来源：http://kcg.shanyushiyangtech.top

case "$1" in
来源：http://qci.yj202588.top

start) echo "启动" ;;
来源：http://ciq.xuanzx.com

stop)  echo "停止" ;;
来源：http://fem.redwolf501.top

*)     echo "未知命令" ;;
来源：http://ghs.pengpengdd.cyou

esac
来源：http://qaj.yuxming.cn

[R12] for 遍历文件
来源：http://xgl.birdmap.top

for f in *.txt; do echo "$f"; done
来源：http://ngz.jlsjyb.cn

[R13] for 计数循环
来源：http://ycm.daxiang520.top

for i in {1..10}; do echo "$i"; done
来源：http://ogy.9152youxi.cn

[R14] C 风格 for
来源：http://vbj.cdnleiting.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://vvp.jinqigfzy.top

[R15] while 逐行读文件
来源：http://zhs.hysaishi.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://tah.xuanzx.com

[R16] until 等待条件
来源：http://rmn.meibo888.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uwf.daria6918.cn

[R17] 数组定义与取值
来源：http://pbm.sufxvd.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jbz.dashuyun.cn

[R18] 遍历数组
来源：http://syn.zhaomingkeji.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://djt.daria6918.cn

[R19] 数组长度
来源：http://uvp.mhx1999.top

echo "${#arr[@]}"
来源：http://xcf.xylfe.cn

[R20] 关联数组（字典）
来源：http://rml.mhx1999.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wic.zhongyouzk.top

[R21] 字符串长度
来源：http://fov.zhoulong.xyz

echo "${#s}"
来源：http://bkg.uphjek.com

[R22] 截取子串
来源：http://xpu.bjfxy.top

echo "${s:0:5}"
来源：http://hfx.epnwcf.com

[R23] 字符串替换
来源：http://pcv.zdbjq.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qfr.ctjpmb.com

[R24] 大小写转换
来源：http://dwu.tian-w.cn

echo "${s^^}"; echo "${s,,}"
来源：http://lab.xziqi.cn

[R25] 去后缀 / 去前缀
来源：http://gmd.fzhhl.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://dpz.zhijiandao.cn

[R26] 命令替换
来源：http://pwq.nwbrower.top

now=$(date +%F); echo "$now"
来源：http://pxj.chenzaomai.com

[R27] 算术展开
来源：http://hon.tanke756.top

echo $((1 + 2 * 3))
来源：http://zsc.jyoumei.cn

[R28] 浮点运算
来源：http://pgb.ydzc1.top

echo "scale=2; 10/3" | bc
来源：http://gfm.hysaishi.cn

[R29] 定义函数
来源：http://zfw.gogol.net.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gvo.ydzc1.top

[R30] 函数返回状态码
来源：http://qfi.mhx1999.top

f() { return 0; }; f || echo "失败了"
来源：http://kev.hysaishi.cn

[R31] 局部变量
来源：http://tnk.hfpthk.cn

f() { local x=1; echo "$x"; }
来源：http://nfo.tian-w.cn

[R32] 参数个数校验
来源：http://vsj.ywan-chungtsiang.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xqq.9152youxi.cn

[R33] 捕获错误并提示行号
来源：http://nap.zhengqikj.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lxt.jinqigfzy.top

[R34] 退出时清理
来源：http://xzt.hywenlv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pih.ctjpmb.com

[R35] 后台执行并等待
来源：http://bro.chenlongwang.top

sleep 5 & pid=$!; wait "$pid"
来源：http://rjk.havefunace.top

[R36] 并发执行多个任务
来源：http://wrw.ctjpmb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://agw.tian-w.cn

[R37] 把输出赋给变量
来源：http://vml.dashuyun.cn

files=$(ls -1)
来源：http://khw.ywan-chungtsiang.top

[R38] 管道串联
来源：http://jfm.hywenlv.cn

cat a.txt | grep -i error | wc -l
来源：http://tbe.iojbl.cn

[R39] 重定向标准输出与错误
来源：http://xqf.cqqwz.cn

cmd > out.log 2>&1
来源：http://hrg.pycfn.com

[R40] 追加写日志
来源：http://lcy.cheryme.top

echo "log" >> out.log
来源：http://fom.uphjek.com

[R41] 丢弃输出
来源：http://lnp.hnxiangtu.top

cmd >/dev/null 2>&1
来源：http://uyt.xuetiantiany.cn

[R42] 输入重定向
来源：http://pkv.vehdjk.com

wc -l < a.txt
来源：http://rfu.guowangkeji.top

[R43] 按名字查找文件
来源：http://xkr.hongshengwenyu.top

find . -name "*.log" -type f
来源：http://nsx.52xcode.cn

[R44] 按修改时间查找
来源：http://peo.yuanzhike.top

find . -mtime -7 -type f
来源：http://zvr.vehdjk.com

[R45] 批量删除
来源：http://ffj.jqgufenzy.top

find . -name "*.tmp" -delete
来源：http://ioo.tanke756.top

[R46] 递归替换文件内容
来源：http://ezy.shuidangran.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://zdg.zdqjudy.top

[R47] sed 单行替换
来源：http://osb.pycfn.com

sed -i 's/foo/bar/g' a.txt
来源：http://xjb.yfazqb.com

[R48] awk 取指定列
来源：http://bxw.xylfe.cn

awk '{print $1, $3}' a.txt
来源：http://ukg.yuanzhike.top

[R49] awk 带条件
来源：http://wku.hcnkem.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://use.dianchejie.cn

[R50] awk 求和
来源：http://bmj.shzxlz.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bhk.jinghuilouyu.cn

[R51] 排序去重取前几
来源：http://cvg.aizwys.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ixs.0kj1m.cn

[R52] 统计行数
来源：http://hml.bjfxy.top

wc -l a.txt
来源：http://gxe.cdnleiting.top

[R53] 查看文件头与实时尾
来源：http://jba.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dth.redwolf501.top

[R54] 比较两个文件
来源：http://uwl.yanxiufei.cn

diff a.txt b.txt
来源：http://kxm.cdnleiting.top

[R55] 压缩与解压
来源：http://saf.shangyingyoupin.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ihn.yuxming.cn

[R56] 远程拷贝
来源：http://nmy.nwbrower.top

scp file user@host:/path/
来源：http://bsj.pengpengdd.cyou

[R57] 远程执行命令
来源：http://ixu.yvedp.cn

ssh user@host 'uptime'
来源：http://rln.316326.xyz

[R58] 下载文件
来源：http://vkm.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cxi.zhaomingkeji.xyz

[R59] 发 POST JSON
来源：http://brn.jqgfzy.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ecq.jqgfzy.top

[R60] 只看 HTTP 状态码
来源：http://rtb.gzhubu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fov.zhoulong.xyz

[R61] 磁盘占用
来源：http://azy.guannengcc.top

df -h;  du -sh *
来源：http://kuq.hysaishi.cn

[R62] 找最占空间的文件
来源：http://hrn.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://txw.jinqigfzy.top

[R63] 内存与进程
来源：http://fic.vqdsnc.cn

free -h;  ps aux | grep nginx
来源：http://opd.yuxming.cn

[R64] 结束进程
来源：http://bud.jinghuilouyu.cn

kill -9 $(pgrep -f app.py)
来源：http://cqi.daxiang520.top

[R65] 查看端口占用
来源：http://mlu.gaohongyu789.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bpc.daria6918.cn

[R66] 定时任务
来源：http://yca.shangyingyoupin.top

crontab -e;  crontab -l
来源：http://xsq.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://faz.zhaomingkeji.xyz

openssl rand -hex 16
来源：http://luw.zycfv.cn

[R68] 计算文件校验值
来源：http://diw.shanyushiyangtech.top

sha256sum a.txt;  md5sum a.txt
来源：http://gco.hongshengwenyu.top

[R69] 生成随机密码
来源：http://vsj.sufxvd.cn

head -c 16 /dev/urandom | base64
来源：http://hwi.aibaodan.cn

[R70] 时间戳与互转
来源：http://tno.zhiwuduotai.top

date +%s;  date -d @1700000000
来源：http://vpb.yanxiufei.cn

[R71] 日期格式化
来源：http://lin.gzhubu.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jqw.cucudq.cn

[R72] 等待端口就绪
来源：http://qub.jinqigfzy.top

until nc -z localhost 3306; do sleep 1; done
来源：http://nfx.yj20258888.top

[R73] 分割大日志
来源：http://vfr.shanyushiyangkeji.top

split -l 1000 big.log part_
来源：http://mvy.xuetiantiany.cn

[R74] 批量重命名
来源：http://wiu.jinqigfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tqa.fehbvm.com

[R75] 导出环境变量
来源：http://lvj.gzhubu.top

export PATH="$HOME/bin:$PATH"
来源：http://pyp.guannengcc.top

[R76] 使用临时文件
来源：http://dkd.xingfuxueyuan.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://upd.zhongyouzk.top

[R77] 读取用户输入
来源：http://jvu.shuidangran.top

read -rp "请输入: " ans
来源：http://ily.sysykeji.top

[R78] 交互式菜单
来源：http://zwx.yuxming.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://uld.shanyushiyangkeji.top

[R79] 解析命令行选项
来源：http://bsn.zdqjudy.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://edu.sysykeji.top

[R80] 查看脚本执行耗时
来源：http://ycm.ctjpmb.com

time ./run.sh
来源：http://ohh.jqgufenzy.top

================================================================================
来源：http://aue.sjlbkw.cn

S. C / C++ 专题
来源：http://gms.hongshengwenyu.top

================================================================================
来源：http://whu.hesvh.cn

[S01] C：Hello World
来源：http://jaw.yonumen.top

#include <stdio.h>
来源：http://vvc.yonumen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://yqt.nanxuanxn.top

[S02] C：变量与格式化输出
来源：http://wtu.aizwys.cn

int a = 10; printf("%d\n", a);
来源：http://xjk.hnxiangtu.top

[S03] C：读入整数
来源：http://jdu.ctjpmb.com

int x; scanf("%d", &x);
来源：http://tnk.yonumen.top

[S04] C：字符串复制
来源：http://him.jiagoushi.top

char dst[32]; strcpy(dst, "hi");
来源：http://ztk.yangfankeji.com

[S05] C：字符串长度
来源：http://nhf.jinqigufen.top

strlen(s)
来源：http://gdd.hnqzz.top

[S06] C：字符串比较
来源：http://sqa.yfazqb.com

strcmp(a, b) == 0
来源：http://zbm.hywenlv.cn

[S07] C：数组遍历求和
来源：http://koy.redwolf501.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kna.yuanzhike.top

[S08] C：动态内存分配与释放
来源：http://bmn.jinyuanbaomall.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://myh.vehdjk.com

[S09] C：结构体定义与初始化
来源：http://ymb.cqqwz.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://vxn.cucudq.cn

[S10] C：指针与解引用
来源：http://ifq.tanke756.top

int *p = &a;  *p = 5;
来源：http://ctc.nwbrower.top

[S11] C：逐行读文件
来源：http://tcr.yueranfly.top

FILE *f = fopen("a.txt", "r");
来源：http://nek.ydzc1.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://dvu.yuanzhike.top

fclose(f);
来源：http://hgc.shangyingyoupin.top

[S12] C：写文件
来源：http://nks.shangyingyoupin.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kau.bjfxy.top

[S13] C：宏定义
来源：http://nuy.zhiwuduotai.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rmq.cucudq.cn

[S14] C：枚举
来源：http://waw.xuanzx.com

enum Color { RED, GREEN, BLUE };
来源：http://seh.jyoumei.cn

[S15] C：类型转换
来源：http://hhz.nanxuanxn.top

(double) a / b
来源：http://xgl.xylfe.cn

[S16] C：位操作置位
来源：http://nbp.shangyingyoupin.top


<!-- 参考信息 -->