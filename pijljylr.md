代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://apv.zhiwuduotai.top

[Q52] 删除指定行
来源：http://mzz.vqdsnc.cn

DELETE FROM users WHERE id = 10;
来源：http://myz.pengpengdd.cyou

[Q53] 按条件删除
来源：http://mbj.jlsjyb.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://ulo.meibo888.top

[Q54] 清空表
来源：http://ekq.gzhubu.top

TRUNCATE TABLE logs;
来源：http://los.zhaomingkeji.xyz

[Q55] 排名（并列占位）
来源：http://wel.gotoacloud.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://gwu.zhongyouzk.top

[Q56] 密集排名（并列不占位）
来源：http://qmy.jinghuilouyu.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://sae.fehbvm.com

[Q57] 行号
来源：http://fjc.tarul.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hjw.meibo888.top

[Q58] 累计求和
来源：http://pyo.ywan-chungtsiang.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://liz.yvedp.cn

[Q59] 分组内累计
来源：http://kaw.hammf.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://aby.nanxinkj.top

[Q60] 取上一行 / 下一行
来源：http://tcm.fehbvm.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://oth.mhx1999.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://vak.jlsjyb.cn

[Q61] 移动平均
来源：http://ihc.tarul.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://pmr.jianghu66.top

[Q62] 分组占比
来源：http://oiw.yonumen.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://beh.yonumen.top

[Q63] 开启事务
来源：http://yrv.fanxiaobao.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://qdi.zdbjq.cn

[Q64] 提交事务
来源：http://hue.9152youxi.cn

COMMIT;
来源：http://twe.xingfuxueyuan.xyz

[Q65] 回滚事务
来源：http://goy.hysaishi.cn

ROLLBACK;
来源：http://dtg.andypj.xyz

[Q66] 行锁查询
来源：http://lrh.ppjwa.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://qjw.andypj.xyz

[Q67] 设置隔离级别
来源：http://zpe.nwbrower.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ueg.aizwys.cn

[Q68] 保存点
来源：http://vxc.yj20258888.top

SAVEPOINT sp1;
来源：http://lrg.tian-w.cn

ROLLBACK TO sp1;
来源：http://ffr.fzhhl.top

[Q69] 查看执行计划
来源：http://ter.quarkkingdee.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://woy.dianchejie.cn

[Q70] 更新统计信息
来源：http://hnk.52xcode.cn

ANALYZE TABLE users;
来源：http://los.jlsjyb.cn

[Q71] 查看建表语句
来源：http://kln.yangfankeji.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://leu.316326.xyz

[Q72] 查看索引
来源：http://oej.zhongyouzk.top

SHOW INDEX FROM users;
来源：http://rkb.yvedp.cn

[Q73] 查看表状态
来源：http://ijx.chenjidiqi.icu

SHOW TABLE STATUS LIKE 'users';
来源：http://cnx.ywan-chungtsiang.top

[Q74] 强制使用索引
来源：http://vmy.yvedp.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ovn.ywan-chungtsiang.top

[Q75] 日期格式化
来源：http://thw.epnwcf.com

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://scm.zdbjq.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uxm.xinyue.icu

[Q76] 按天统计
来源：http://xky.snrcjt.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ytx.gogol.net.cn

[Q77] 时间加减
来源：http://zxn.9152youxi.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mcc.vqdsnc.cn

[Q78] 当前时间
来源：http://lgw.chenzaomai.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://zqf.chenlongwang.top

[Q79] 字符串拼接
来源：http://etj.fzhhl.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://yfc.nanxinkj.top

[Q80] 字符串截取
来源：http://tnq.nanxuanxn.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gsa.bbcook.cn

[Q81] 字符串替换
来源：http://dcp.chenlongwang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rza.meibo888.top

[Q82] 字符长度与字节长度
来源：http://ila.chenjidiqi.icu

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://oqj.vqdsnc.cn

[Q83] 大小写转换
来源：http://sjp.zhixingplan.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kzl.daxiang520.top

[Q84] 去除首尾空格
来源：http://fcv.jianghu66.top

SELECT TRIM(name) FROM users;
来源：http://qyd.hesvh.cn

[Q85] 数值取整
来源：http://cxd.feifeiyinyue.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://vhl.ivvv.top

[Q86] 读取 JSON 字段
来源：http://ypc.ppjwa.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mub.chenlongwang.top

[Q87] JSON 字段做条件
来源：http://ssd.jqgfzy.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ong.daxiang520.top

[Q88] 行转列（条件聚合）
来源：http://fta.xingfuxueyuan.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rgc.tanke756.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qte.sweek.top

[Q89] 判断表是否存在
来源：http://xpk.jinqigfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xli.yongpay.top

[Q90] 生成序号列
来源：http://vhb.hcnkem.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://sji.gogol.net.cn

================================================================================
来源：http://nob.guannengcc.top

R. Bash 专题
来源：http://lmx.zhaomingkeji.xyz

================================================================================
来源：http://hod.gotoacloud.top

[R01] shebang 与严格模式
来源：http://efp.iojbl.cn

#!/usr/bin/env bash
来源：http://yhy.guannengcc.top

set -euo pipefail
来源：http://fbh.cqqwz.cn

[R02] 变量赋值与使用
来源：http://axa.daria6918.cn

name="Tom"; echo "$name"
来源：http://gip.nanxinkj.top

[R03] 只读变量
来源：http://rdy.chenjidiqi.icu

readonly PI=3.14
来源：http://ovg.gotoacloud.top

[R04] 位置参数
来源：http://ywv.jqgfzy.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://tly.hongshengwenyu.top

[R05] 参数默认值
来源：http://efj.zdbjq.cn

name="${1:-default}"
来源：http://iaq.jinyuanbaomall.cn

[R06] 判断命令是否存在
来源：http://kzh.gotoacloud.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://skr.vqdsnc.cn

[R07] if 判断文件
来源：http://nzb.fzhhl.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hbm.wangshuangyany.cn

[R08] 数值比较
来源：http://hid.feifeiyinyue.top

if (( a > b )); then echo "a 更大"; fi
来源：http://yfr.pycfn.com

[R09] 字符串比较
来源：http://ltu.ywan-chungtsiang.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xbp.zdbjq.cn

[R10] 正则匹配
来源：http://maq.guowangkeji.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nab.iojbl.cn

[R11] case 多分支
来源：http://yem.ywan-chungtsiang.top

case "$1" in
来源：http://nov.cashguo.top

start) echo "启动" ;;
来源：http://ezv.shzxlz.cn

stop)  echo "停止" ;;
来源：http://dfv.zhijiandao.cn

*)     echo "未知命令" ;;
来源：http://bsf.sufxvd.cn

esac
来源：http://fee.xingfuxueyuan.xyz

[R12] for 遍历文件
来源：http://pdn.jinghuilouyu.cn

for f in *.txt; do echo "$f"; done
来源：http://kun.shanyushiyangtech.top

[R13] for 计数循环
来源：http://hgt.52xcode.cn

for i in {1..10}; do echo "$i"; done
来源：http://jnd.sufxvd.cn

[R14] C 风格 for
来源：http://ubn.yongpay.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ntd.52xcode.cn

[R15] while 逐行读文件
来源：http://osp.ivvv.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://oid.nanxuanxn.top

[R16] until 等待条件
来源：http://rqv.dashuyun.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://uwq.cashguo.top

[R17] 数组定义与取值
来源：http://qbv.yanxiufei.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kvu.yueranfly.top

[R18] 遍历数组
来源：http://lwa.jinqigfzy.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ena.yj20258.top

[R19] 数组长度
来源：http://qwd.zycfv.cn

echo "${#arr[@]}"
来源：http://nph.jlsjyb.cn

[R20] 关联数组（字典）
来源：http://viv.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xeu.andypj.xyz

[R21] 字符串长度
来源：http://ohd.gotoacloud.top

echo "${#s}"
来源：http://jyk.haohaochexian.top

[R22] 截取子串
来源：http://ium.52xcode.cn

echo "${s:0:5}"
来源：http://bjq.yfazqb.com

[R23] 字符串替换
来源：http://swr.jyoumei.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://skh.gotoacloud.top

[R24] 大小写转换
来源：http://ulf.vehdjk.com

echo "${s^^}"; echo "${s,,}"
来源：http://unb.xziqi.cn

[R25] 去后缀 / 去前缀
来源：http://hyz.jiagoushi.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://ain.jyoumei.cn

[R26] 命令替换
来源：http://qrv.zhiwuduotai.top

now=$(date +%F); echo "$now"
来源：http://wqr.sysykeji.top

[R27] 算术展开
来源：http://eds.xuanzx.com

echo $((1 + 2 * 3))
来源：http://cky.iojbl.cn

[R28] 浮点运算
来源：http://yyo.dashuyun.cn

echo "scale=2; 10/3" | bc
来源：http://uuv.tianlin.xyz

[R29] 定义函数
来源：http://ecs.fanxiaobao.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cmx.hcnkem.com

[R30] 函数返回状态码
来源：http://yak.tarul.cn

f() { return 0; }; f || echo "失败了"
来源：http://hey.zhongyouzk.top

[R31] 局部变量
来源：http://azq.havefunace.top

f() { local x=1; echo "$x"; }
来源：http://lme.birdmap.top

[R32] 参数个数校验
来源：http://jie.daria6918.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://vlh.cashguo.top

[R33] 捕获错误并提示行号
来源：http://lck.hesvh.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dvt.316326.xyz

[R34] 退出时清理
来源：http://ntz.yuanzhike.top

trap 'rm -f "$tmp"' EXIT
来源：http://vlm.chenjidiqi.icu

[R35] 后台执行并等待
来源：http://uli.tarul.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fzb.tarul.cn

[R36] 并发执行多个任务
来源：http://qup.tarul.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tts.feifeiyinyue.top

[R37] 把输出赋给变量
来源：http://drn.sjlbkw.cn

files=$(ls -1)
来源：http://dzj.ydzc1.top

[R38] 管道串联
来源：http://yxq.smart0.xyz

cat a.txt | grep -i error | wc -l
来源：http://fwg.gaohongyu789.top

[R39] 重定向标准输出与错误
来源：http://fal.dianchejie.cn

cmd > out.log 2>&1
来源：http://upi.ydzc1.top

[R40] 追加写日志
来源：http://thx.zdbjq.cn

echo "log" >> out.log
来源：http://oky.xuetiantiany.cn

[R41] 丢弃输出
来源：http://ecb.shangyingyoupin.top

cmd >/dev/null 2>&1
来源：http://tec.epnwcf.com

[R42] 输入重定向
来源：http://gow.quarkkingdee.top

wc -l < a.txt
来源：http://zdk.chenlongwang.top

[R43] 按名字查找文件
来源：http://ctp.gogol.net.cn

find . -name "*.log" -type f
来源：http://yqz.jinyuanbaomall.cn

[R44] 按修改时间查找
来源：http://bba.vqdsnc.cn

find . -mtime -7 -type f
来源：http://kcg.hysaishi.cn

[R45] 批量删除
来源：http://nqn.quarkkingdee.top

find . -name "*.tmp" -delete
来源：http://sax.jianghu66.top

[R46] 递归替换文件内容
来源：http://acy.cqqwz.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hvp.hongshengwenyu.top

[R47] sed 单行替换
来源：http://eis.yj202588.top

sed -i 's/foo/bar/g' a.txt
来源：http://oai.hywenlv.cn

[R48] awk 取指定列
来源：http://jrr.andypj.xyz

awk '{print $1, $3}' a.txt
来源：http://sll.hammf.cn

[R49] awk 带条件
来源：http://qjq.cqqwz.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ygs.tianlin.xyz

[R50] awk 求和
来源：http://twt.xingfuxueyuan.xyz

awk '{s += $2} END {print s}' a.txt
来源：http://zdu.yj20258.top

[R51] 排序去重取前几
来源：http://wla.cucudq.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rwq.hcnkem.com

[R52] 统计行数
来源：http://tbp.chenlongwang.top

wc -l a.txt
来源：http://agp.haohaochexian.top

[R53] 查看文件头与实时尾
来源：http://lma.wangshuangyany.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://lzj.svipenyu.cn

[R54] 比较两个文件
来源：http://sro.snrcjt.cn

diff a.txt b.txt
来源：http://hel.nanxuanxn.top

[R55] 压缩与解压
来源：http://jum.smart0.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://cqz.gzhubu.top

[R56] 远程拷贝
来源：http://hoh.jqgfzy.top

scp file user@host:/path/
来源：http://rrj.chenjidiqi.icu

[R57] 远程执行命令
来源：http://azr.zhoulong.xyz

ssh user@host 'uptime'
来源：http://oub.yvedp.cn

[R58] 下载文件
来源：http://ztt.jqgfzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://myr.epnwcf.com

[R59] 发 POST JSON
来源：http://vwh.9152youxi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mgo.xuanzx.com

[R60] 只看 HTTP 状态码
来源：http://ltx.cdnleiting.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lst.shangyingyoupin.top

[R61] 磁盘占用
来源：http://myz.feifeiyinyue.top

df -h;  du -sh *
来源：http://ifn.ctjpmb.com

[R62] 找最占空间的文件
来源：http://mhd.c1oappe.top

du -ah . | sort -rh | head -10
来源：http://iac.fktsv.cn

[R63] 内存与进程
来源：http://tkl.cqqwz.cn

free -h;  ps aux | grep nginx
来源：http://pcx.ehwqpu.com

[R64] 结束进程
来源：http://bkn.shuidangran.top

kill -9 $(pgrep -f app.py)
来源：http://xxk.xziqi.cn

[R65] 查看端口占用
来源：http://tjm.dashuyun.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vqs.yueranfly.top

[R66] 定时任务
来源：http://tem.ehwqpu.com

crontab -e;  crontab -l
来源：http://zly.0kj1m.cn

[R67] 生成随机十六进制串
来源：http://qff.yj20258888.top

openssl rand -hex 16
来源：http://ddi.sjlbkw.cn

[R68] 计算文件校验值
来源：http://gnu.jianghu66.top

sha256sum a.txt;  md5sum a.txt
来源：http://ssw.xylfe.cn

[R69] 生成随机密码
来源：http://wgi.yueranfly.top

head -c 16 /dev/urandom | base64
来源：http://xdv.sweek.top

[R70] 时间戳与互转
来源：http://uxi.snrcjt.cn

date +%s;  date -d @1700000000
来源：http://pwa.quarkkingdee.top

[R71] 日期格式化
来源：http://zba.dashuyun.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lkx.52xcode.cn

[R72] 等待端口就绪
来源：http://ign.yangfankeji.com

until nc -z localhost 3306; do sleep 1; done
来源：http://dzy.feifeiyinyue.top

[R73] 分割大日志
来源：http://ihb.nanxinkj.top

split -l 1000 big.log part_
来源：http://fbf.jiagoushi.top

[R74] 批量重命名
来源：http://syt.ybcxt.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wkr.zycfv.cn

[R75] 导出环境变量
来源：http://ekm.shangyingyoupin.top

export PATH="$HOME/bin:$PATH"
来源：http://kyz.sysykeji.top

[R76] 使用临时文件
来源：http://ams.0kj1m.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yhq.ydjk.org.cn

[R77] 读取用户输入
来源：http://pct.cashguo.top

read -rp "请输入: " ans
来源：http://puk.shzxlz.cn

[R78] 交互式菜单
来源：http://pxc.redwolf501.top

select opt in a b c; do echo "$opt"; break; done
来源：http://mgp.hnqzz.top

[R79] 解析命令行选项
来源：http://nry.yj20258888.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wjc.andypj.xyz

[R80] 查看脚本执行耗时
来源：http://wja.uphjek.com

time ./run.sh
来源：http://yvo.chenzaomai.com

================================================================================
来源：http://brg.fanxiaobao.xyz

S. C / C++ 专题
来源：http://jpc.jlsjyb.cn

================================================================================
来源：http://cfw.hywenlv.cn

[S01] C：Hello World
来源：http://qvb.yuanzhike.top

#include <stdio.h>
来源：http://uma.yvedp.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hzb.svipenyu.cn

[S02] C：变量与格式化输出
来源：http://asd.andypj.xyz

int a = 10; printf("%d\n", a);
来源：http://fir.chenzaomai.com

[S03] C：读入整数
来源：http://nnr.feifeiyinyue.top

int x; scanf("%d", &x);
来源：http://qul.fzhhl.top

[S04] C：字符串复制
来源：http://xpf.daria6918.cn

char dst[32]; strcpy(dst, "hi");
来源：http://oci.svipenyu.cn

[S05] C：字符串长度
来源：http://qtv.c1oappe.top

strlen(s)
来源：http://asu.fengsongda.top

[S06] C：字符串比较
来源：http://zre.hnqzz.top

strcmp(a, b) == 0
来源：http://cqu.chenjidiqi.icu

[S07] C：数组遍历求和
来源：http://ukt.hammf.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jqj.sufxvd.cn

[S08] C：动态内存分配与释放
来源：http://vuq.pengpengdd.cyou

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ydu.birdmap.top

[S09] C：结构体定义与初始化
来源：http://pkl.yvedp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uvc.yongpay.top

[S10] C：指针与解引用
来源：http://whm.fanxiaobao.xyz

int *p = &a;  *p = 5;
来源：http://rlz.zycfv.cn

[S11] C：逐行读文件
来源：http://hlj.tian-w.cn

FILE *f = fopen("a.txt", "r");
来源：http://nvs.jyoumei.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jtf.316326.xyz

fclose(f);
来源：http://tpr.zhijiandao.cn

[S12] C：写文件
来源：http://ylp.hongshengwenyu.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kpm.hongshengwenyu.top

[S13] C：宏定义
来源：http://znz.ppjwa.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://twr.meibo888.top

[S14] C：枚举
来源：http://gps.yueranfly.top

enum Color { RED, GREEN, BLUE };
来源：http://nsy.xuanzx.com

[S15] C：类型转换
来源：http://elw.mhx1999.top

(double) a / b
来源：http://esm.yj20258888.top

[S16] C：位操作置位
来源：http://ggo.sxryk.cn

x |= (1 << 3);
来源：http://nen.aibaodan.cn

[S17] C：安全拼接字符串
来源：http://nxy.gaohongyu789.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bkn.zycfv.cn

[S18] C：命令行参数
来源：http://iex.gogol.net.cn

int main(int argc, char **argv)
来源：http://tys.hnxiangtu.top

[S19] C：快速排序
来源：http://bgh.dianchejie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kyc.hcnkem.com

[S20] C：二分查找
来源：http://spa.ppjwa.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yjm.hongshengwenyu.top

[S21] C：字符类别判断
来源：http://clo.smart0.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jzr.jinqigfzy.top

[S22] C：字符串转数字
来源：http://ntp.guowangkeji.top


<!-- 参考信息 -->