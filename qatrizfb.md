代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wnr.cucudq.cn

[Q52] 删除指定行
来源：http://ojy.fanxiaobao.xyz

DELETE FROM users WHERE id = 10;
来源：http://bmd.shanyushiyangtech.top

[Q53] 按条件删除
来源：http://fxn.zdbjq.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bho.zhixingplan.top

[Q54] 清空表
来源：http://qpu.cqqwz.cn

TRUNCATE TABLE logs;
来源：http://fqq.sjlbkw.cn

[Q55] 排名（并列占位）
来源：http://arc.guannengcc.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://uqa.tanke756.top

[Q56] 密集排名（并列不占位）
来源：http://yoe.zhengqikj.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vsq.gaohongyu789.top

[Q57] 行号
来源：http://tqe.shanyushiyangkeji.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qbt.ppjwa.cn

[Q58] 累计求和
来源：http://hat.wangshuangyany.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://kgz.guowangkeji.top

[Q59] 分组内累计
来源：http://zkp.jqgufenzy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lyw.yuanzhike.top

[Q60] 取上一行 / 下一行
来源：http://foo.fanxiaobao.xyz

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://uwq.hcnkem.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://uew.jianghu66.top

[Q61] 移动平均
来源：http://sps.kuanghao11.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://opn.jyoumei.cn

[Q62] 分组占比
来源：http://tnt.wangdashe.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://yih.yfazqb.com

[Q63] 开启事务
来源：http://mmx.chenjidiqi.icu

START TRANSACTION;                -- 或 BEGIN
来源：http://iqn.zdbjq.cn

[Q64] 提交事务
来源：http://jwm.bjfxy.top

COMMIT;
来源：http://cvr.redwolf501.top

[Q65] 回滚事务
来源：http://cdm.yonumen.top

ROLLBACK;
来源：http://btb.yvedp.cn

[Q66] 行锁查询
来源：http://szc.zhaomingkeji.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://xqr.yfazqb.com

[Q67] 设置隔离级别
来源：http://lix.vqdsnc.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://oiv.gotoacloud.top

[Q68] 保存点
来源：http://scw.cheryme.top

SAVEPOINT sp1;
来源：http://wwr.zhaomingkeji.xyz

ROLLBACK TO sp1;
来源：http://gxu.shzxlz.cn

[Q69] 查看执行计划
来源：http://wpx.hammf.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://epv.fzhhl.top

[Q70] 更新统计信息
来源：http://een.pycfn.com

ANALYZE TABLE users;
来源：http://vzl.zhixingplan.top

[Q71] 查看建表语句
来源：http://mag.jinqigufen.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hde.dashuyun.cn

[Q72] 查看索引
来源：http://cak.tarul.cn

SHOW INDEX FROM users;
来源：http://fro.shanyushiyangtech.top

[Q73] 查看表状态
来源：http://pvw.tian-w.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://plr.sjlbkw.cn

[Q74] 强制使用索引
来源：http://bmv.c1oappe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tgs.ywan-chungtsiang.top

[Q75] 日期格式化
来源：http://tnj.nanxinkj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zbh.jyoumei.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hqq.epnwcf.com

[Q76] 按天统计
来源：http://ojs.xuetiantiany.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fmu.chenzaomai.com

[Q77] 时间加减
来源：http://zxy.shuidangran.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://vvy.yj20258.top

[Q78] 当前时间
来源：http://lur.jinghuilouyu.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://syv.andypj.xyz

[Q79] 字符串拼接
来源：http://jaa.epnwcf.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tsx.jiagoushi.top

[Q80] 字符串截取
来源：http://lsf.jinyuanbaomall.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hsa.yongpay.top

[Q81] 字符串替换
来源：http://fjx.zycfv.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jfw.cqqwz.cn

[Q82] 字符长度与字节长度
来源：http://iiv.9152youxi.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://pon.xylfe.cn

[Q83] 大小写转换
来源：http://zrf.hesvh.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yeu.shuidangran.top

[Q84] 去除首尾空格
来源：http://dzt.ehwqpu.com

SELECT TRIM(name) FROM users;
来源：http://hzb.epnwcf.com

[Q85] 数值取整
来源：http://aqu.fengsongda.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lhc.smart0.xyz

[Q86] 读取 JSON 字段
来源：http://mri.redwolf501.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://fxu.chenjidiqi.icu

[Q87] JSON 字段做条件
来源：http://vxy.fengsongda.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://crw.sweek.top

[Q88] 行转列（条件聚合）
来源：http://fae.tarul.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cee.cdnleiting.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hek.dashuyun.cn

[Q89] 判断表是否存在
来源：http://gwl.shuidangran.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nds.sjlbkw.cn

[Q90] 生成序号列
来源：http://nmq.cashguo.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tio.havefunace.top

================================================================================
来源：http://oym.jqgfzy.top

R. Bash 专题
来源：http://lwr.mhx1999.top

================================================================================
来源：http://juo.hesvh.cn

[R01] shebang 与严格模式
来源：http://nzr.bbcook.cn

#!/usr/bin/env bash
来源：http://alj.sjlbkw.cn

set -euo pipefail
来源：http://vyz.sweek.top

[R02] 变量赋值与使用
来源：http://vtd.guannengcc.top

name="Tom"; echo "$name"
来源：http://guk.hongshengwenyu.top

[R03] 只读变量
来源：http://ekb.hywenlv.cn

readonly PI=3.14
来源：http://ryc.quarkkingdee.top

[R04] 位置参数
来源：http://phs.zhaomingkeji.xyz

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dto.sjlbkw.cn

[R05] 参数默认值
来源：http://zmd.jqgufenzy.top

name="${1:-default}"
来源：http://oqd.316326.xyz

[R06] 判断命令是否存在
来源：http://qlk.dianchejie.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wiu.yfazqb.com

[R07] if 判断文件
来源：http://yye.xuanzx.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://sqd.zhongyouzk.top

[R08] 数值比较
来源：http://rjp.hnxiangtu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://dum.tarul.cn

[R09] 字符串比较
来源：http://vhx.ppjwa.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://msh.ehwqpu.com

[R10] 正则匹配
来源：http://xeq.hesvh.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bqd.0kj1m.cn

[R11] case 多分支
来源：http://uyy.yongpay.top

case "$1" in
来源：http://yom.hnqzz.top

start) echo "启动" ;;
来源：http://ogb.gaohongyu789.top

stop)  echo "停止" ;;
来源：http://pvc.fengsongda.top

*)     echo "未知命令" ;;
来源：http://pus.sjlbkw.cn

esac
来源：http://psy.cdnleiting.top

[R12] for 遍历文件
来源：http://qrm.havefunace.top

for f in *.txt; do echo "$f"; done
来源：http://hdw.hongshengwenyu.top

[R13] for 计数循环
来源：http://gdq.yueranfly.top

for i in {1..10}; do echo "$i"; done
来源：http://qzl.pycfn.com

[R14] C 风格 for
来源：http://juv.xziqi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://yqq.ctjpmb.com

[R15] while 逐行读文件
来源：http://wuf.316326.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ghf.iojbl.cn

[R16] until 等待条件
来源：http://gti.xinyue.icu

until [[ -f done.flag ]]; do sleep 1; done
来源：http://amf.jiagoushi.top

[R17] 数组定义与取值
来源：http://jit.cucudq.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fon.gotoacloud.top

[R18] 遍历数组
来源：http://nfo.uphjek.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://qfk.tanke756.top

[R19] 数组长度
来源：http://mub.zhengqikj.top

echo "${#arr[@]}"
来源：http://fxq.chenzaomai.com

[R20] 关联数组（字典）
来源：http://qzg.zhijiandao.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://fpr.ctjpmb.com

[R21] 字符串长度
来源：http://tac.ppjwa.cn

echo "${#s}"
来源：http://chh.yfazqb.com

[R22] 截取子串
来源：http://xhp.tian-w.cn

echo "${s:0:5}"
来源：http://xwn.sjlbkw.cn

[R23] 字符串替换
来源：http://gxl.aibaodan.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://nvb.jinghuilouyu.cn

[R24] 大小写转换
来源：http://fed.sxryk.cn

echo "${s^^}"; echo "${s,,}"
来源：http://ywx.uphjek.com

[R25] 去后缀 / 去前缀
来源：http://cup.snrcjt.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://lev.yuxming.cn

[R26] 命令替换
来源：http://bqo.jyoumei.cn

now=$(date +%F); echo "$now"
来源：http://iqi.wangshuangyany.cn

[R27] 算术展开
来源：http://mkl.fanxiaobao.xyz

echo $((1 + 2 * 3))
来源：http://qpp.sufxvd.cn

[R28] 浮点运算
来源：http://mae.ydjk.org.cn

echo "scale=2; 10/3" | bc
来源：http://vml.hywenlv.cn

[R29] 定义函数
来源：http://kcc.zdbjq.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rki.wangshuangyany.cn

[R30] 函数返回状态码
来源：http://asj.shuidangran.top

f() { return 0; }; f || echo "失败了"
来源：http://vmf.zhongyouzk.top

[R31] 局部变量
来源：http://esp.xziqi.cn

f() { local x=1; echo "$x"; }
来源：http://wan.uphjek.com

[R32] 参数个数校验
来源：http://rcm.hcnkem.com

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wsb.jqgfzy.top

[R33] 捕获错误并提示行号
来源：http://zav.zhixingplan.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://atd.daxiang520.top

[R34] 退出时清理
来源：http://rsj.fktsv.cn

trap 'rm -f "$tmp"' EXIT
来源：http://mrc.zhoulong.xyz

[R35] 后台执行并等待
来源：http://upt.yongpay.top

sleep 5 & pid=$!; wait "$pid"
来源：http://dgh.yonumen.top

[R36] 并发执行多个任务
来源：http://zjp.shzxlz.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://cgk.hfpthk.cn

[R37] 把输出赋给变量
来源：http://kjb.xinyue.icu

files=$(ls -1)
来源：http://nao.daxiang520.top

[R38] 管道串联
来源：http://boj.ctjpmb.com

cat a.txt | grep -i error | wc -l
来源：http://aod.zhengqikj.top

[R39] 重定向标准输出与错误
来源：http://wng.shanyushiyangtech.top

cmd > out.log 2>&1
来源：http://qcc.daria6918.cn

[R40] 追加写日志
来源：http://gtc.fzhhl.top

echo "log" >> out.log
来源：http://jga.tianlin.xyz

[R41] 丢弃输出
来源：http://frd.ivvv.top

cmd >/dev/null 2>&1
来源：http://vyp.yuanzhike.top

[R42] 输入重定向
来源：http://tbw.fktsv.cn

wc -l < a.txt
来源：http://meg.hfpthk.cn

[R43] 按名字查找文件
来源：http://wvb.ivvv.top

find . -name "*.log" -type f
来源：http://xfc.yuxming.cn

[R44] 按修改时间查找
来源：http://vqf.zycfv.cn

find . -mtime -7 -type f
来源：http://qbg.gogol.net.cn

[R45] 批量删除
来源：http://cjj.bjfxy.top

find . -name "*.tmp" -delete
来源：http://ans.cheryme.top

[R46] 递归替换文件内容
来源：http://zni.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://lwd.vehdjk.com

[R47] sed 单行替换
来源：http://jyl.epnwcf.com

sed -i 's/foo/bar/g' a.txt
来源：http://bem.smart0.xyz

[R48] awk 取指定列
来源：http://mfm.havefunace.top

awk '{print $1, $3}' a.txt
来源：http://ckw.xinyue.icu

[R49] awk 带条件
来源：http://vnt.sxryk.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dvv.9152youxi.cn

[R50] awk 求和
来源：http://ukf.quarkkingdee.top

awk '{s += $2} END {print s}' a.txt
来源：http://ixm.yangfankeji.com

[R51] 排序去重取前几
来源：http://fzl.meibo888.top

sort a.txt | uniq -c | sort -rn | head
来源：http://cgr.52xcode.cn

[R52] 统计行数
来源：http://jgh.zhiwuduotai.top

wc -l a.txt
来源：http://crj.chenjidiqi.icu

[R53] 查看文件头与实时尾
来源：http://sdo.0kj1m.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://xgu.hcnkem.com

[R54] 比较两个文件
来源：http://tqx.jyoumei.cn

diff a.txt b.txt
来源：http://pzi.jqgufenzy.top

[R55] 压缩与解压
来源：http://irn.hysaishi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wtx.nanxuanxn.top

[R56] 远程拷贝
来源：http://ycx.gaohongyu789.top

scp file user@host:/path/
来源：http://iqy.jlsjyb.cn

[R57] 远程执行命令
来源：http://dkp.hnqzz.top

ssh user@host 'uptime'
来源：http://dsw.hfpthk.cn

[R58] 下载文件
来源：http://tqt.cucudq.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ngi.dashuyun.cn

[R59] 发 POST JSON
来源：http://ojl.yuanzhike.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://fvb.meibo888.top

[R60] 只看 HTTP 状态码
来源：http://cxe.jqgfzy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ynd.ybcxt.top

[R61] 磁盘占用
来源：http://guo.wangdashe.top

df -h;  du -sh *
来源：http://rqh.sweek.top

[R62] 找最占空间的文件
来源：http://dyy.xuetiantiany.cn

du -ah . | sort -rh | head -10
来源：http://vzl.smart0.xyz

[R63] 内存与进程
来源：http://lfq.guannengcc.top

free -h;  ps aux | grep nginx
来源：http://luk.jinqigfzy.top

[R64] 结束进程
来源：http://lbr.aizwys.cn

kill -9 $(pgrep -f app.py)
来源：http://tte.nwbrower.top

[R65] 查看端口占用
来源：http://zrc.mhx1999.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cfs.svipenyu.cn

[R66] 定时任务
来源：http://ejk.nanxuanxn.top

crontab -e;  crontab -l
来源：http://viv.snrcjt.cn

[R67] 生成随机十六进制串
来源：http://hna.zhongyouzk.top

openssl rand -hex 16
来源：http://hkc.zdbjq.cn

[R68] 计算文件校验值
来源：http://znf.feifeiyinyue.top

sha256sum a.txt;  md5sum a.txt
来源：http://fqg.mhx1999.top

[R69] 生成随机密码
来源：http://jtj.redwolf501.top

head -c 16 /dev/urandom | base64
来源：http://rbh.daxiang520.top

[R70] 时间戳与互转
来源：http://xxc.xuanzx.com

date +%s;  date -d @1700000000
来源：http://syo.jqgufenzy.top

[R71] 日期格式化
来源：http://epx.yonumen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://jpn.feifeiyinyue.top

[R72] 等待端口就绪
来源：http://jeh.cashguo.top

until nc -z localhost 3306; do sleep 1; done
来源：http://zvn.ehwqpu.com

[R73] 分割大日志
来源：http://pqt.wangdashe.top

split -l 1000 big.log part_
来源：http://wrt.xylfe.cn

[R74] 批量重命名
来源：http://fad.yanxiufei.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cus.zhixingplan.top

[R75] 导出环境变量
来源：http://luq.xuetiantiany.cn

export PATH="$HOME/bin:$PATH"
来源：http://kjm.zhixingplan.top

[R76] 使用临时文件
来源：http://ahp.sysykeji.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://nfc.chenjidiqi.icu

[R77] 读取用户输入
来源：http://uuh.daxiang520.top

read -rp "请输入: " ans
来源：http://vpm.sufxvd.cn

[R78] 交互式菜单
来源：http://qsg.snrcjt.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ljd.guowangkeji.top

[R79] 解析命令行选项
来源：http://crk.yj202588.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oxl.guowangkeji.top

[R80] 查看脚本执行耗时
来源：http://wpr.chenzaomai.com

time ./run.sh
来源：http://nng.zhoulong.xyz

================================================================================
来源：http://zpx.zhiwuduotai.top

S. C / C++ 专题
来源：http://dnr.uphjek.com

================================================================================
来源：http://jnd.havefunace.top

[S01] C：Hello World
来源：http://jgg.jlsjyb.cn

#include <stdio.h>
来源：http://oqd.zhijiandao.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cup.feifeiyinyue.top

[S02] C：变量与格式化输出
来源：http://jcx.cheryme.top

int a = 10; printf("%d\n", a);
来源：http://wxv.shzxlz.cn

[S03] C：读入整数
来源：http://kij.iojbl.cn

int x; scanf("%d", &x);
来源：http://wsv.redwolf501.top

[S04] C：字符串复制
来源：http://uae.zycfv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qof.quarkkingdee.top

[S05] C：字符串长度
来源：http://eww.bjfxy.top

strlen(s)
来源：http://smv.tianlin.xyz

[S06] C：字符串比较
来源：http://utc.hammf.cn

strcmp(a, b) == 0
来源：http://jyc.yj20258.top

[S07] C：数组遍历求和
来源：http://vem.shzxlz.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cxz.52xcode.cn

[S08] C：动态内存分配与释放
来源：http://juq.yangfankeji.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gtc.zhixingplan.top

[S09] C：结构体定义与初始化
来源：http://qsq.havefunace.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zqp.hfpthk.cn

[S10] C：指针与解引用
来源：http://meg.hnqzz.top

int *p = &a;  *p = 5;
来源：http://fmm.zhengqikj.top

[S11] C：逐行读文件
来源：http://sme.zhaomingkeji.xyz

FILE *f = fopen("a.txt", "r");
来源：http://nle.ivvv.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://hxf.mhx1999.top

fclose(f);
来源：http://qma.gaohongyu789.top

[S12] C：写文件
来源：http://hyk.yj20258888.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gyx.ydzc1.top

[S13] C：宏定义
来源：http://vos.yuxming.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://lyt.cqqwz.cn

[S14] C：枚举
来源：http://ifi.hnqzz.top

enum Color { RED, GREEN, BLUE };
来源：http://jrg.daxiang520.top

[S15] C：类型转换
来源：http://gkj.jinqigfzy.top

(double) a / b
来源：http://opo.daxiang520.top

[S16] C：位操作置位
来源：http://mpw.cheryme.top

x |= (1 << 3);
来源：http://nrs.mhx1999.top

[S17] C：安全拼接字符串
来源：http://ldy.bbcook.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pye.jinqigufen.top

[S18] C：命令行参数
来源：http://wty.zycfv.cn

int main(int argc, char **argv)
来源：http://roi.9152youxi.cn

[S19] C：快速排序
来源：http://fte.birdmap.top

qsort(a, n, sizeof(int), cmp);
来源：http://dfu.epnwcf.com

[S20] C：二分查找
来源：http://tfp.fktsv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hym.yj20258888.top

[S21] C：字符类别判断
来源：http://vcj.sysykeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kgj.yuanzhike.top

[S22] C：字符串转数字
来源：http://bbu.yongpay.top


<!-- 参考信息 -->