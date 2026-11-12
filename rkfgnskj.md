代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://iml.tarul.cn

[Q52] 删除指定行
来源：http://mio.jqgfzy.top

DELETE FROM users WHERE id = 10;
来源：http://zil.yuxming.cn

[Q53] 按条件删除
来源：http://oat.jinghuilouyu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jrk.guowangkeji.top

[Q54] 清空表
来源：http://eew.yangfankeji.com

TRUNCATE TABLE logs;
来源：http://ndu.hysaishi.cn

[Q55] 排名（并列占位）
来源：http://qyk.yuxming.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://ovi.cheryme.top

[Q56] 密集排名（并列不占位）
来源：http://uqp.feifeiyinyue.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ude.yanxiufei.cn

[Q57] 行号
来源：http://ovj.hnxiangtu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://rwa.haohaochexian.top

[Q58] 累计求和
来源：http://xan.ctjpmb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vuk.jqgfzy.top

[Q59] 分组内累计
来源：http://iwt.yvedp.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://bwm.ivvv.top

[Q60] 取上一行 / 下一行
来源：http://esr.yuanzhike.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cqt.kuanghao11.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://gvc.nanxinkj.top

[Q61] 移动平均
来源：http://pnf.jianghu66.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://ngc.dashuyun.cn

[Q62] 分组占比
来源：http://ewt.jinqigfzy.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://goc.cucudq.cn

[Q63] 开启事务
来源：http://gtk.guowangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://puy.nanxuanxn.top

[Q64] 提交事务
来源：http://gne.sjlbkw.cn

COMMIT;
来源：http://fgd.cucudq.cn

[Q65] 回滚事务
来源：http://stt.kuanghao11.cn

ROLLBACK;
来源：http://ybi.aizwys.cn

[Q66] 行锁查询
来源：http://qrb.andypj.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wbi.dashuyun.cn

[Q67] 设置隔离级别
来源：http://whq.316326.xyz

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://adi.wangshuangyany.cn

[Q68] 保存点
来源：http://qrx.fktsv.cn

SAVEPOINT sp1;
来源：http://tou.ybcxt.top

ROLLBACK TO sp1;
来源：http://bgu.0kj1m.cn

[Q69] 查看执行计划
来源：http://uez.dianchejie.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://gri.tarul.cn

[Q70] 更新统计信息
来源：http://foy.iojbl.cn

ANALYZE TABLE users;
来源：http://hud.chenlongwang.top

[Q71] 查看建表语句
来源：http://taf.zhoulong.xyz

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://poa.kuanghao11.cn

[Q72] 查看索引
来源：http://ybr.chenzaomai.com

SHOW INDEX FROM users;
来源：http://gow.ehwqpu.com

[Q73] 查看表状态
来源：http://jbw.cucudq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://oqr.redwolf501.top

[Q74] 强制使用索引
来源：http://qbm.fktsv.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ple.fanxiaobao.xyz

[Q75] 日期格式化
来源：http://kxg.chenzaomai.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://cau.shzxlz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xwr.chenzaomai.com

[Q76] 按天统计
来源：http://rsk.zdbjq.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cup.yvedp.cn

[Q77] 时间加减
来源：http://iir.9152youxi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nzx.yuxming.cn

[Q78] 当前时间
来源：http://fzh.zhengqikj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jgx.jinyuanbaomall.cn

[Q79] 字符串拼接
来源：http://zvu.cucudq.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cwc.smart0.xyz

[Q80] 字符串截取
来源：http://afi.fzhhl.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uim.guowangkeji.top

[Q81] 字符串替换
来源：http://vmi.dianchejie.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pfc.ppjwa.cn

[Q82] 字符长度与字节长度
来源：http://wda.uphjek.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pqr.cucudq.cn

[Q83] 大小写转换
来源：http://gnw.xingfuxueyuan.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sxl.zhongyouzk.top

[Q84] 去除首尾空格
来源：http://xja.daxiang520.top

SELECT TRIM(name) FROM users;
来源：http://lar.jinyuanbaomall.cn

[Q85] 数值取整
来源：http://jae.meibo888.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://fqu.c1oappe.top

[Q86] 读取 JSON 字段
来源：http://axb.wangdashe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://cag.yanxiufei.cn

[Q87] JSON 字段做条件
来源：http://yee.cashguo.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kbp.mhx1999.top

[Q88] 行转列（条件聚合）
来源：http://pgz.meibo888.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hvs.chenjidiqi.icu

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wxt.kuanghao11.cn

[Q89] 判断表是否存在
来源：http://fvz.yj202588.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jkg.fzhhl.top

[Q90] 生成序号列
来源：http://zjc.epnwcf.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://zex.hammf.cn

================================================================================
来源：http://pxy.xuetiantiany.cn

R. Bash 专题
来源：http://dbw.jinyuanbaomall.cn

================================================================================
来源：http://hkb.wangshuangyany.cn

[R01] shebang 与严格模式
来源：http://run.sjlbkw.cn

#!/usr/bin/env bash
来源：http://gxv.jinghuilouyu.cn

set -euo pipefail
来源：http://reh.sysykeji.top

[R02] 变量赋值与使用
来源：http://wwh.pengpengdd.cyou

name="Tom"; echo "$name"
来源：http://bzb.gzhubu.top

[R03] 只读变量
来源：http://ohj.guannengcc.top

readonly PI=3.14
来源：http://geg.daxiang520.top

[R04] 位置参数
来源：http://toc.zhaomingkeji.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vok.ivvv.top

[R05] 参数默认值
来源：http://fpe.shanyushiyangkeji.top

name="${1:-default}"
来源：http://pvh.shzxlz.cn

[R06] 判断命令是否存在
来源：http://veq.meibo888.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://sfa.yj20258888.top

[R07] if 判断文件
来源：http://reg.yonumen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bde.jyoumei.cn

[R08] 数值比较
来源：http://xye.wangshuangyany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://aul.gogol.net.cn

[R09] 字符串比较
来源：http://rxe.chenzaomai.com

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qts.yuanzhike.top

[R10] 正则匹配
来源：http://xys.havefunace.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nul.kuanghao11.cn

[R11] case 多分支
来源：http://nqt.vehdjk.com

case "$1" in
来源：http://zag.ydjk.org.cn

start) echo "启动" ;;
来源：http://hls.haohaochexian.top

stop)  echo "停止" ;;
来源：http://wjp.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://fro.sjlbkw.cn

esac
来源：http://vqh.chenjidiqi.icu

[R12] for 遍历文件
来源：http://kdt.hammf.cn

for f in *.txt; do echo "$f"; done
来源：http://lbc.vqdsnc.cn

[R13] for 计数循环
来源：http://xwh.yanxiufei.cn

for i in {1..10}; do echo "$i"; done
来源：http://zei.bbcook.cn

[R14] C 风格 for
来源：http://oul.ppjwa.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jxy.shangyingyoupin.top

[R15] while 逐行读文件
来源：http://krg.hywenlv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://awi.aibaodan.cn

[R16] until 等待条件
来源：http://btf.chenjidiqi.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://jic.gzhubu.top

[R17] 数组定义与取值
来源：http://ecw.vehdjk.com

arr=(a b c); echo "${arr[0]}"
来源：http://yka.aibaodan.cn

[R18] 遍历数组
来源：http://zqt.zdbjq.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://kqx.shangyingyoupin.top

[R19] 数组长度
来源：http://pjy.hnxiangtu.top

echo "${#arr[@]}"
来源：http://mzc.ppjwa.cn

[R20] 关联数组（字典）
来源：http://xfv.guowangkeji.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://vno.xziqi.cn

[R21] 字符串长度
来源：http://mea.hongshengwenyu.top

echo "${#s}"
来源：http://tjm.kuanghao11.cn

[R22] 截取子串
来源：http://ddx.gzhubu.top

echo "${s:0:5}"
来源：http://bum.hcnkem.com

[R23] 字符串替换
来源：http://bhq.ydjk.org.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dri.hnqzz.top

[R24] 大小写转换
来源：http://xcy.yonumen.top

echo "${s^^}"; echo "${s,,}"
来源：http://pdr.yj20258.top

[R25] 去后缀 / 去前缀
来源：http://fsv.nanxinkj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://nuc.smart0.xyz

[R26] 命令替换
来源：http://jsv.hywenlv.cn

now=$(date +%F); echo "$now"
来源：http://wmz.iojbl.cn

[R27] 算术展开
来源：http://hxz.jlsjyb.cn

echo $((1 + 2 * 3))
来源：http://due.quarkkingdee.top

[R28] 浮点运算
来源：http://bes.ydjk.org.cn

echo "scale=2; 10/3" | bc
来源：http://wwp.zhiwuduotai.top

[R29] 定义函数
来源：http://dik.vehdjk.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gsm.bbcook.cn

[R30] 函数返回状态码
来源：http://cir.xinyue.icu

f() { return 0; }; f || echo "失败了"
来源：http://rrl.yonumen.top

[R31] 局部变量
来源：http://yia.gzhubu.top

f() { local x=1; echo "$x"; }
来源：http://wfl.yanxiufei.cn

[R32] 参数个数校验
来源：http://duh.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tql.c1oappe.top

[R33] 捕获错误并提示行号
来源：http://ohs.redwolf501.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rty.uphjek.com

[R34] 退出时清理
来源：http://hip.shzxlz.cn

trap 'rm -f "$tmp"' EXIT
来源：http://pac.iojbl.cn

[R35] 后台执行并等待
来源：http://jzw.zycfv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://gqd.yangfankeji.com

[R36] 并发执行多个任务
来源：http://aug.zhixingplan.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://did.aizwys.cn

[R37] 把输出赋给变量
来源：http://lmm.9152youxi.cn

files=$(ls -1)
来源：http://ytf.guannengcc.top

[R38] 管道串联
来源：http://ynh.yonumen.top

cat a.txt | grep -i error | wc -l
来源：http://msz.yfazqb.com

[R39] 重定向标准输出与错误
来源：http://wtg.yonumen.top

cmd > out.log 2>&1
来源：http://wow.ybcxt.top

[R40] 追加写日志
来源：http://rcs.fzhhl.top

echo "log" >> out.log
来源：http://iua.fktsv.cn

[R41] 丢弃输出
来源：http://twd.shanyushiyangtech.top

cmd >/dev/null 2>&1
来源：http://osk.jinghuilouyu.cn

[R42] 输入重定向
来源：http://evq.zhixingplan.top

wc -l < a.txt
来源：http://oaz.haohaochexian.top

[R43] 按名字查找文件
来源：http://rnw.iojbl.cn

find . -name "*.log" -type f
来源：http://fhi.yvedp.cn

[R44] 按修改时间查找
来源：http://swi.pycfn.com

find . -mtime -7 -type f
来源：http://rov.zhixingplan.top

[R45] 批量删除
来源：http://cxq.c1oappe.top

find . -name "*.tmp" -delete
来源：http://tir.shanyushiyangkeji.top

[R46] 递归替换文件内容
来源：http://syj.xylfe.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ipe.guannengcc.top

[R47] sed 单行替换
来源：http://khv.hcnkem.com

sed -i 's/foo/bar/g' a.txt
来源：http://lcz.yuxming.cn

[R48] awk 取指定列
来源：http://pjt.bjfxy.top

awk '{print $1, $3}' a.txt
来源：http://qqi.jqgfzy.top

[R49] awk 带条件
来源：http://bzz.jlsjyb.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cpw.yanxiufei.cn

[R50] awk 求和
来源：http://fra.zhengqikj.top

awk '{s += $2} END {print s}' a.txt
来源：http://uix.hcnkem.com

[R51] 排序去重取前几
来源：http://fmj.jyoumei.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vez.smart0.xyz

[R52] 统计行数
来源：http://hyf.ehwqpu.com

wc -l a.txt
来源：http://itr.xylfe.cn

[R53] 查看文件头与实时尾
来源：http://mcy.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nkh.ywan-chungtsiang.top

[R54] 比较两个文件
来源：http://bgg.jiagoushi.top

diff a.txt b.txt
来源：http://jaa.yangfankeji.com

[R55] 压缩与解压
来源：http://usa.andypj.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://qcm.zhengqikj.top

[R56] 远程拷贝
来源：http://svw.shuidangran.top

scp file user@host:/path/
来源：http://das.ywan-chungtsiang.top

[R57] 远程执行命令
来源：http://bcq.cucudq.cn

ssh user@host 'uptime'
来源：http://ndy.ydjk.org.cn

[R58] 下载文件
来源：http://sma.zhoulong.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://riv.nwbrower.top

[R59] 发 POST JSON
来源：http://ihf.jinghuilouyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qng.0kj1m.cn

[R60] 只看 HTTP 状态码
来源：http://ieh.yangfankeji.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gpc.aizwys.cn

[R61] 磁盘占用
来源：http://qnl.c1oappe.top

df -h;  du -sh *
来源：http://xxb.feifeiyinyue.top

[R62] 找最占空间的文件
来源：http://afl.daria6918.cn

du -ah . | sort -rh | head -10
来源：http://hxq.jqgufenzy.top

[R63] 内存与进程
来源：http://wxy.xingfuxueyuan.xyz

free -h;  ps aux | grep nginx
来源：http://lps.zhongyouzk.top

[R64] 结束进程
来源：http://wum.fktsv.cn

kill -9 $(pgrep -f app.py)
来源：http://skh.daria6918.cn

[R65] 查看端口占用
来源：http://arw.316326.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://nfl.0kj1m.cn

[R66] 定时任务
来源：http://gdx.52xcode.cn

crontab -e;  crontab -l
来源：http://rey.jinqigfzy.top

[R67] 生成随机十六进制串
来源：http://vaf.shanyushiyangkeji.top

openssl rand -hex 16
来源：http://yas.nanxinkj.top

[R68] 计算文件校验值
来源：http://mub.9152youxi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://app.sufxvd.cn

[R69] 生成随机密码
来源：http://pvk.daxiang520.top

head -c 16 /dev/urandom | base64
来源：http://xgy.epnwcf.com

[R70] 时间戳与互转
来源：http://dxo.mhx1999.top

date +%s;  date -d @1700000000
来源：http://mkf.52xcode.cn

[R71] 日期格式化
来源：http://doo.jinghuilouyu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ivn.hcnkem.com

[R72] 等待端口就绪
来源：http://qst.bbcook.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ihg.hammf.cn

[R73] 分割大日志
来源：http://roy.nanxuanxn.top

split -l 1000 big.log part_
来源：http://ynx.hnxiangtu.top

[R74] 批量重命名
来源：http://arj.chenjidiqi.icu

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yzc.xylfe.cn

[R75] 导出环境变量
来源：http://vqw.gogol.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://kba.jyoumei.cn

[R76] 使用临时文件
来源：http://xpt.birdmap.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://crf.redwolf501.top

[R77] 读取用户输入
来源：http://ycj.bbcook.cn

read -rp "请输入: " ans
来源：http://llh.xuetiantiany.cn

[R78] 交互式菜单
来源：http://tca.xziqi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dif.jyoumei.cn

[R79] 解析命令行选项
来源：http://kgq.zhijiandao.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wuz.fanxiaobao.xyz

[R80] 查看脚本执行耗时
来源：http://bfj.nanxinkj.top

time ./run.sh
来源：http://lgo.ywan-chungtsiang.top

================================================================================
来源：http://zrn.cdnleiting.top

S. C / C++ 专题
来源：http://qhs.wangshuangyany.cn

================================================================================
来源：http://hjy.guannengcc.top

[S01] C：Hello World
来源：http://trk.vqdsnc.cn

#include <stdio.h>
来源：http://mai.haohaochexian.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://naf.zhengqikj.top

[S02] C：变量与格式化输出
来源：http://czj.guannengcc.top

int a = 10; printf("%d\n", a);
来源：http://snl.sxryk.cn

[S03] C：读入整数
来源：http://ocs.0kj1m.cn

int x; scanf("%d", &x);
来源：http://spc.redwolf501.top

[S04] C：字符串复制
来源：http://jqh.cqqwz.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wbl.sxryk.cn

[S05] C：字符串长度
来源：http://knx.hcnkem.com

strlen(s)
来源：http://wzq.jlsjyb.cn

[S06] C：字符串比较
来源：http://xqe.jinqigufen.top

strcmp(a, b) == 0
来源：http://nlv.haohaochexian.top

[S07] C：数组遍历求和
来源：http://vbj.zhiwuduotai.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wmf.sjlbkw.cn

[S08] C：动态内存分配与释放
来源：http://vdm.uphjek.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gue.chenjidiqi.icu

[S09] C：结构体定义与初始化
来源：http://wta.tianlin.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pqy.yvedp.cn

[S10] C：指针与解引用
来源：http://pss.pengpengdd.cyou

int *p = &a;  *p = 5;
来源：http://jrc.zhengqikj.top

[S11] C：逐行读文件
来源：http://qed.zdbjq.cn

FILE *f = fopen("a.txt", "r");
来源：http://mnh.epnwcf.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://quq.vehdjk.com

fclose(f);
来源：http://ygy.xinyue.icu

[S12] C：写文件
来源：http://cve.fktsv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mrs.hywenlv.cn

[S13] C：宏定义
来源：http://dxg.kuanghao11.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://njm.guannengcc.top

[S14] C：枚举
来源：http://fhi.svipenyu.cn

enum Color { RED, GREEN, BLUE };
来源：http://tyh.aizwys.cn

[S15] C：类型转换
来源：http://szr.sxryk.cn

(double) a / b
来源：http://pkt.jyoumei.cn

[S16] C：位操作置位
来源：http://rli.xuanzx.com

x |= (1 << 3);
来源：http://raq.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://bnw.shuidangran.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bpc.tian-w.cn

[S18] C：命令行参数
来源：http://asi.316326.xyz

int main(int argc, char **argv)
来源：http://idm.sweek.top

[S19] C：快速排序
来源：http://ttv.chenjidiqi.icu

qsort(a, n, sizeof(int), cmp);
来源：http://tqx.uphjek.com

[S20] C：二分查找
来源：http://biy.daria6918.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://amu.yonumen.top

[S21] C：字符类别判断
来源：http://nms.gzhubu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://odq.c1oappe.top

[S22] C：字符串转数字
来源：http://lyi.jianghu66.top


<!-- 参考信息 -->