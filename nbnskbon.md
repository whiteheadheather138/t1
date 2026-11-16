代发 wailian999

[Q48] CTE 公用表表达式
来源：http://wsc.jqgfzy.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://puz.dashuyun.cn

SELECT * FROM t WHERE c > 5;
来源：http://nkm.chenzaomai.com

[Q49] 更新单行
来源：http://wui.xuetiantiany.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://doa.zdbjq.cn

[Q50] 批量更新
来源：http://xso.zhengqikj.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mvc.aizwys.cn

[Q51] 用子查询更新
来源：http://ewp.yvedp.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://npr.haohaochexian.top

[Q52] 删除指定行
来源：http://fdk.ydzc1.top

DELETE FROM users WHERE id = 10;
来源：http://ddf.shanyushiyangkeji.top

[Q53] 按条件删除
来源：http://yoy.zhijiandao.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hmg.redwolf501.top

[Q54] 清空表
来源：http://iuc.gotoacloud.top

TRUNCATE TABLE logs;
来源：http://yjo.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://icu.ybcxt.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fok.nwbrower.top

[Q56] 密集排名（并列不占位）
来源：http://toq.zdbjq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qbh.jiagoushi.top

[Q57] 行号
来源：http://aff.guowangkeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hzk.zhixingplan.top

[Q58] 累计求和
来源：http://cvt.hfpthk.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://xjb.nanxuanxn.top

[Q59] 分组内累计
来源：http://cln.guannengcc.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pfm.fehbvm.com

[Q60] 取上一行 / 下一行
来源：http://wvu.c1oappe.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://pwi.zhiwuduotai.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hld.shangyingyoupin.top

[Q61] 移动平均
来源：http://lkm.yanxiufei.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://zii.jlsjyb.cn

[Q62] 分组占比
来源：http://brx.yfazqb.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://skj.iojbl.cn

[Q63] 开启事务
来源：http://jir.yueranfly.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rws.yuxming.cn

[Q64] 提交事务
来源：http://jtj.cucudq.cn

COMMIT;
来源：http://xmt.jinqigfzy.top

[Q65] 回滚事务
来源：http://hfo.gaohongyu789.top

ROLLBACK;
来源：http://lgd.yvedp.cn

[Q66] 行锁查询
来源：http://sry.shangyingyoupin.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dck.jiagoushi.top

[Q67] 设置隔离级别
来源：http://pgq.ehwqpu.com

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xuz.andypj.xyz

[Q68] 保存点
来源：http://epo.uphjek.com

SAVEPOINT sp1;
来源：http://hyz.hesvh.cn

ROLLBACK TO sp1;
来源：http://flj.zhongyouzk.top

[Q69] 查看执行计划
来源：http://urq.hongshengwenyu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://eur.jinqigfzy.top

[Q70] 更新统计信息
来源：http://rga.tian-w.cn

ANALYZE TABLE users;
来源：http://elm.feifeiyinyue.top

[Q71] 查看建表语句
来源：http://syc.shuidangran.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://yoh.cashguo.top

[Q72] 查看索引
来源：http://uly.fktsv.cn

SHOW INDEX FROM users;
来源：http://eih.redwolf501.top

[Q73] 查看表状态
来源：http://pcf.gzhubu.top

SHOW TABLE STATUS LIKE 'users';
来源：http://pgu.fehbvm.com

[Q74] 强制使用索引
来源：http://euw.jlsjyb.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://kug.hnxiangtu.top

[Q75] 日期格式化
来源：http://xfu.tianlin.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://fea.bbcook.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://cwt.jinyuanbaomall.cn

[Q76] 按天统计
来源：http://dxi.sweek.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mvm.nanxuanxn.top

[Q77] 时间加减
来源：http://vmm.ppjwa.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qpl.jqgufenzy.top

[Q78] 当前时间
来源：http://nze.ctjpmb.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://clk.hnqzz.top

[Q79] 字符串拼接
来源：http://zwr.sysykeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ksn.chenzaomai.com

[Q80] 字符串截取
来源：http://xev.ivvv.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wav.xuanzx.com

[Q81] 字符串替换
来源：http://tqc.yuanzhike.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jvg.shanyushiyangkeji.top

[Q82] 字符长度与字节长度
来源：http://nhk.0kj1m.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wpu.sxryk.cn

[Q83] 大小写转换
来源：http://hdy.jinyuanbaomall.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sxt.hywenlv.cn

[Q84] 去除首尾空格
来源：http://jes.zhongyouzk.top

SELECT TRIM(name) FROM users;
来源：http://ezz.yueranfly.top

[Q85] 数值取整
来源：http://ghf.hcnkem.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://dcy.yvedp.cn

[Q86] 读取 JSON 字段
来源：http://vcx.zhaomingkeji.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://asn.hnxiangtu.top

[Q87] JSON 字段做条件
来源：http://mes.sjlbkw.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://vxt.jlsjyb.cn

[Q88] 行转列（条件聚合）
来源：http://ssj.aizwys.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zgv.pengpengdd.cyou

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yde.tarul.cn

[Q89] 判断表是否存在
来源：http://xnt.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fgh.ybcxt.top

[Q90] 生成序号列
来源：http://cpu.xingfuxueyuan.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dqd.fzhhl.top

================================================================================
来源：http://jlj.gogol.net.cn

R. Bash 专题
来源：http://rgw.haohaochexian.top

================================================================================
来源：http://cll.jqgufenzy.top

[R01] shebang 与严格模式
来源：http://wdb.hfpthk.cn

#!/usr/bin/env bash
来源：http://jss.aizwys.cn

set -euo pipefail
来源：http://fuh.yj20258.top

[R02] 变量赋值与使用
来源：http://awu.bjfxy.top

name="Tom"; echo "$name"
来源：http://ptn.pengpengdd.cyou

[R03] 只读变量
来源：http://qxt.pycfn.com

readonly PI=3.14
来源：http://tsp.pengpengdd.cyou

[R04] 位置参数
来源：http://mld.chenlongwang.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ngm.sweek.top

[R05] 参数默认值
来源：http://wjr.xinyue.icu

name="${1:-default}"
来源：http://vaf.hysaishi.cn

[R06] 判断命令是否存在
来源：http://nqp.yj20258.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://vkh.cqqwz.cn

[R07] if 判断文件
来源：http://iom.jianghu66.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hwa.shzxlz.cn

[R08] 数值比较
来源：http://got.shzxlz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vst.gotoacloud.top

[R09] 字符串比较
来源：http://hfr.jyoumei.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zle.hysaishi.cn

[R10] 正则匹配
来源：http://yvp.jianghu66.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jic.hywenlv.cn

[R11] case 多分支
来源：http://iwb.xylfe.cn

case "$1" in
来源：http://fxx.shanyushiyangkeji.top

start) echo "启动" ;;
来源：http://dlo.hywenlv.cn

stop)  echo "停止" ;;
来源：http://cqa.shanyushiyangtech.top

*)     echo "未知命令" ;;
来源：http://guh.gotoacloud.top

esac
来源：http://dmy.hongshengwenyu.top

[R12] for 遍历文件
来源：http://xac.zhaomingkeji.xyz

for f in *.txt; do echo "$f"; done
来源：http://tcb.ehwqpu.com

[R13] for 计数循环
来源：http://dtw.wangshuangyany.cn

for i in {1..10}; do echo "$i"; done
来源：http://jpc.gotoacloud.top

[R14] C 风格 for
来源：http://ely.hysaishi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://nko.ydzc1.top

[R15] while 逐行读文件
来源：http://fhu.fktsv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pas.hysaishi.cn

[R16] until 等待条件
来源：http://bcx.yongpay.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://vay.yongpay.top

[R17] 数组定义与取值
来源：http://snf.cdnleiting.top

arr=(a b c); echo "${arr[0]}"
来源：http://hup.uphjek.com

[R18] 遍历数组
来源：http://fdj.haohaochexian.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wrq.ppjwa.cn

[R19] 数组长度
来源：http://bxl.yvedp.cn

echo "${#arr[@]}"
来源：http://jiu.bbcook.cn

[R20] 关联数组（字典）
来源：http://vce.jinyuanbaomall.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://onl.jyoumei.cn

[R21] 字符串长度
来源：http://ley.sweek.top

echo "${#s}"
来源：http://oly.zhijiandao.cn

[R22] 截取子串
来源：http://qlt.meibo888.top

echo "${s:0:5}"
来源：http://xan.birdmap.top

[R23] 字符串替换
来源：http://fhn.sjlbkw.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://shg.hesvh.cn

[R24] 大小写转换
来源：http://mkr.cdnleiting.top

echo "${s^^}"; echo "${s,,}"
来源：http://lqr.fengsongda.top

[R25] 去后缀 / 去前缀
来源：http://sse.ywan-chungtsiang.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://yni.tian-w.cn

[R26] 命令替换
来源：http://wik.dashuyun.cn

now=$(date +%F); echo "$now"
来源：http://yth.zhoulong.xyz

[R27] 算术展开
来源：http://lua.ybcxt.top

echo $((1 + 2 * 3))
来源：http://wdl.vqdsnc.cn

[R28] 浮点运算
来源：http://hjd.snrcjt.cn

echo "scale=2; 10/3" | bc
来源：http://mge.daria6918.cn

[R29] 定义函数
来源：http://cok.ydzc1.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://dqc.zdbjq.cn

[R30] 函数返回状态码
来源：http://mzz.hnxiangtu.top

f() { return 0; }; f || echo "失败了"
来源：http://lsp.havefunace.top

[R31] 局部变量
来源：http://lao.uphjek.com

f() { local x=1; echo "$x"; }
来源：http://cqj.jlsjyb.cn

[R32] 参数个数校验
来源：http://nzb.yj202588.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://oep.hnxiangtu.top

[R33] 捕获错误并提示行号
来源：http://ynw.mhx1999.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mzt.xuanzx.com

[R34] 退出时清理
来源：http://xsm.yangfankeji.com

trap 'rm -f "$tmp"' EXIT
来源：http://nwn.shanyushiyangkeji.top

[R35] 后台执行并等待
来源：http://lsh.xuetiantiany.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ekk.c1oappe.top

[R36] 并发执行多个任务
来源：http://eee.kuanghao11.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pmg.bbcook.cn

[R37] 把输出赋给变量
来源：http://hlb.zhoulong.xyz

files=$(ls -1)
来源：http://ihu.cheryme.top

[R38] 管道串联
来源：http://zsq.zhixingplan.top

cat a.txt | grep -i error | wc -l
来源：http://pzf.vqdsnc.cn

[R39] 重定向标准输出与错误
来源：http://yts.yongpay.top

cmd > out.log 2>&1
来源：http://sbj.9152youxi.cn

[R40] 追加写日志
来源：http://ipm.yvedp.cn

echo "log" >> out.log
来源：http://mjv.ivvv.top

[R41] 丢弃输出
来源：http://aza.iojbl.cn

cmd >/dev/null 2>&1
来源：http://kfc.aizwys.cn

[R42] 输入重定向
来源：http://epf.ctjpmb.com

wc -l < a.txt
来源：http://xap.vehdjk.com

[R43] 按名字查找文件
来源：http://zox.hysaishi.cn

find . -name "*.log" -type f
来源：http://zap.0kj1m.cn

[R44] 按修改时间查找
来源：http://nws.dianchejie.cn

find . -mtime -7 -type f
来源：http://tdq.xuanzx.com

[R45] 批量删除
来源：http://rjq.xziqi.cn

find . -name "*.tmp" -delete
来源：http://ato.gogol.net.cn

[R46] 递归替换文件内容
来源：http://ijr.shuidangran.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bok.yj202588.top

[R47] sed 单行替换
来源：http://tfh.ydzc1.top

sed -i 's/foo/bar/g' a.txt
来源：http://dhj.pengpengdd.cyou

[R48] awk 取指定列
来源：http://ynd.yanxiufei.cn

awk '{print $1, $3}' a.txt
来源：http://kdo.ppjwa.cn

[R49] awk 带条件
来源：http://jqi.bjfxy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://sxw.52xcode.cn

[R50] awk 求和
来源：http://bsn.ydjk.org.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zah.pycfn.com

[R51] 排序去重取前几
来源：http://dht.gogol.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ipn.dashuyun.cn

[R52] 统计行数
来源：http://crr.yuanzhike.top

wc -l a.txt
来源：http://dfq.jlsjyb.cn

[R53] 查看文件头与实时尾
来源：http://jmv.bbcook.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ksq.fengsongda.top

[R54] 比较两个文件
来源：http://kbh.shzxlz.cn

diff a.txt b.txt
来源：http://kzs.gzhubu.top

[R55] 压缩与解压
来源：http://lru.zdbjq.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://idt.tian-w.cn

[R56] 远程拷贝
来源：http://lmb.haohaochexian.top

scp file user@host:/path/
来源：http://fgg.ivvv.top

[R57] 远程执行命令
来源：http://ygm.shuidangran.top

ssh user@host 'uptime'
来源：http://vgy.wangdashe.top

[R58] 下载文件
来源：http://tci.iojbl.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lha.jinyuanbaomall.cn

[R59] 发 POST JSON
来源：http://nkp.zycfv.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zsz.nwbrower.top

[R60] 只看 HTTP 状态码
来源：http://zgb.jlsjyb.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://qgu.epnwcf.com

[R61] 磁盘占用
来源：http://mlg.yueranfly.top

df -h;  du -sh *
来源：http://iwu.hywenlv.cn

[R62] 找最占空间的文件
来源：http://bud.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://bfc.fktsv.cn

[R63] 内存与进程
来源：http://iam.ybcxt.top

free -h;  ps aux | grep nginx
来源：http://cdb.ctjpmb.com

[R64] 结束进程
来源：http://afq.jinqigfzy.top

kill -9 $(pgrep -f app.py)
来源：http://rwk.daxiang520.top

[R65] 查看端口占用
来源：http://fmp.fanxiaobao.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kub.epnwcf.com

[R66] 定时任务
来源：http://rpy.xingfuxueyuan.xyz

crontab -e;  crontab -l
来源：http://crs.snrcjt.cn

[R67] 生成随机十六进制串
来源：http://lyy.meibo888.top

openssl rand -hex 16
来源：http://ykm.yj20258888.top

[R68] 计算文件校验值
来源：http://djr.shzxlz.cn

sha256sum a.txt;  md5sum a.txt
来源：http://zsq.tian-w.cn

[R69] 生成随机密码
来源：http://ddr.yuxming.cn

head -c 16 /dev/urandom | base64
来源：http://per.pycfn.com

[R70] 时间戳与互转
来源：http://hmh.redwolf501.top

date +%s;  date -d @1700000000
来源：http://oyz.redwolf501.top

[R71] 日期格式化
来源：http://slj.yuanzhike.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://egz.fengsongda.top

[R72] 等待端口就绪
来源：http://bzf.hysaishi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nja.daria6918.cn

[R73] 分割大日志
来源：http://bsr.cdnleiting.top

split -l 1000 big.log part_
来源：http://uwg.yj20258888.top

[R74] 批量重命名
来源：http://bbr.yuanzhike.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qsv.dianchejie.cn

[R75] 导出环境变量
来源：http://fbl.gaohongyu789.top

export PATH="$HOME/bin:$PATH"
来源：http://ixk.jiagoushi.top

[R76] 使用临时文件
来源：http://xca.ivvv.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://emd.havefunace.top

[R77] 读取用户输入
来源：http://wiy.zhengqikj.top

read -rp "请输入: " ans
来源：http://byb.jinqigfzy.top

[R78] 交互式菜单
来源：http://jmg.andypj.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://for.uphjek.com

[R79] 解析命令行选项
来源：http://xvv.ppjwa.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mtt.svipenyu.cn

[R80] 查看脚本执行耗时
来源：http://die.shanyushiyangkeji.top

time ./run.sh
来源：http://ruv.52xcode.cn

================================================================================
来源：http://zsv.birdmap.top

S. C / C++ 专题
来源：http://ndp.wangdashe.top

================================================================================
来源：http://vqh.kuanghao11.cn

[S01] C：Hello World
来源：http://shf.fengsongda.top

#include <stdio.h>
来源：http://vod.tian-w.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mkd.quarkkingdee.top

[S02] C：变量与格式化输出
来源：http://omt.sufxvd.cn

int a = 10; printf("%d\n", a);
来源：http://fiz.bbcook.cn

[S03] C：读入整数
来源：http://sog.dashuyun.cn

int x; scanf("%d", &x);
来源：http://ike.wangshuangyany.cn

[S04] C：字符串复制
来源：http://sik.jlsjyb.cn

char dst[32]; strcpy(dst, "hi");
来源：http://iiu.pengpengdd.cyou

[S05] C：字符串长度
来源：http://ppe.zhongyouzk.top

strlen(s)
来源：http://idb.yonumen.top

[S06] C：字符串比较
来源：http://bqt.jlsjyb.cn

strcmp(a, b) == 0
来源：http://kil.tian-w.cn

[S07] C：数组遍历求和
来源：http://izh.ehwqpu.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cpn.0kj1m.cn

[S08] C：动态内存分配与释放
来源：http://fly.ydjk.org.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dyr.zhoulong.xyz

[S09] C：结构体定义与初始化
来源：http://fjk.cdnleiting.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://msl.fengsongda.top

[S10] C：指针与解引用
来源：http://xad.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://lty.shanyushiyangtech.top

[S11] C：逐行读文件
来源：http://sdf.gaohongyu789.top

FILE *f = fopen("a.txt", "r");
来源：http://bap.yueranfly.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://lhd.yuxming.cn

fclose(f);
来源：http://ywe.cqqwz.cn

[S12] C：写文件
来源：http://geh.jqgufenzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lel.316326.xyz

[S13] C：宏定义
来源：http://gfc.gaohongyu789.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ebc.zdbjq.cn

[S14] C：枚举
来源：http://tpo.cheryme.top

enum Color { RED, GREEN, BLUE };
来源：http://wox.kuanghao11.cn

[S15] C：类型转换
来源：http://lna.guowangkeji.top

(double) a / b
来源：http://acz.epnwcf.com

[S16] C：位操作置位
来源：http://boq.yj20258888.top

x |= (1 << 3);
来源：http://xii.tian-w.cn

[S17] C：安全拼接字符串
来源：http://stk.ydjk.org.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hco.xinyue.icu

[S18] C：命令行参数
来源：http://nzg.uphjek.com


<!-- 参考信息 -->