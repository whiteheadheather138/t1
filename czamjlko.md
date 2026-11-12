代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yzn.9152youxi.cn

[Q50] 批量更新
来源：http://jat.yanxiufei.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://eax.hnqzz.top

[Q51] 用子查询更新
来源：http://dgj.iojbl.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://cyo.iojbl.cn

[Q52] 删除指定行
来源：http://tve.fktsv.cn

DELETE FROM users WHERE id = 10;
来源：http://ytw.yj20258888.top

[Q53] 按条件删除
来源：http://ksb.nwbrower.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://bxr.cqqwz.cn

[Q54] 清空表
来源：http://ron.yj202588.top

TRUNCATE TABLE logs;
来源：http://nhe.hfpthk.cn

[Q55] 排名（并列占位）
来源：http://oiw.guannengcc.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://sjv.0kj1m.cn

[Q56] 密集排名（并列不占位）
来源：http://vlv.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ari.hywenlv.cn

[Q57] 行号
来源：http://nxv.ctjpmb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mwv.andypj.xyz

[Q58] 累计求和
来源：http://suz.gaohongyu789.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://emy.gogol.net.cn

[Q59] 分组内累计
来源：http://fia.svipenyu.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://xvl.ctjpmb.com

[Q60] 取上一行 / 下一行
来源：http://smj.yanxiufei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hsj.jyoumei.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fku.tarul.cn

[Q61] 移动平均
来源：http://qqi.gotoacloud.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tbo.shanyushiyangtech.top

[Q62] 分组占比
来源：http://egi.feifeiyinyue.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://kdw.pengpengdd.cyou

[Q63] 开启事务
来源：http://jnw.jlsjyb.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://zni.fzhhl.top

[Q64] 提交事务
来源：http://tmn.pengpengdd.cyou

COMMIT;
来源：http://qwn.sxryk.cn

[Q65] 回滚事务
来源：http://nit.aibaodan.cn

ROLLBACK;
来源：http://boi.yj20258888.top

[Q66] 行锁查询
来源：http://ouq.jinghuilouyu.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tis.tanke756.top

[Q67] 设置隔离级别
来源：http://vqf.fzhhl.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://iyf.meibo888.top

[Q68] 保存点
来源：http://mdm.yongpay.top

SAVEPOINT sp1;
来源：http://clf.svipenyu.cn

ROLLBACK TO sp1;
来源：http://jnq.dashuyun.cn

[Q69] 查看执行计划
来源：http://zqn.jqgufenzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://myd.jinqigufen.top

[Q70] 更新统计信息
来源：http://ouy.jinyuanbaomall.cn

ANALYZE TABLE users;
来源：http://rgm.zhijiandao.cn

[Q71] 查看建表语句
来源：http://fif.hnqzz.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://owz.fengsongda.top

[Q72] 查看索引
来源：http://cts.yuanzhike.top

SHOW INDEX FROM users;
来源：http://mef.hnqzz.top

[Q73] 查看表状态
来源：http://bzb.aizwys.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://vkc.ydjk.org.cn

[Q74] 强制使用索引
来源：http://tvr.bjfxy.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ned.sxryk.cn

[Q75] 日期格式化
来源：http://jsr.yj20258.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ziu.gzhubu.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://dee.shuidangran.top

[Q76] 按天统计
来源：http://vot.xziqi.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dln.guannengcc.top

[Q77] 时间加减
来源：http://lrb.hnqzz.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://iwm.xylfe.cn

[Q78] 当前时间
来源：http://bef.zhengqikj.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lus.daria6918.cn

[Q79] 字符串拼接
来源：http://wkx.jqgufenzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gmi.316326.xyz

[Q80] 字符串截取
来源：http://ris.gaohongyu789.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://rnu.jianghu66.top

[Q81] 字符串替换
来源：http://yqa.yuanzhike.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://qpc.snrcjt.cn

[Q82] 字符长度与字节长度
来源：http://tje.hesvh.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lrt.havefunace.top

[Q83] 大小写转换
来源：http://mjq.ybcxt.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://piw.sjlbkw.cn

[Q84] 去除首尾空格
来源：http://afj.fktsv.cn

SELECT TRIM(name) FROM users;
来源：http://gmh.hcnkem.com

[Q85] 数值取整
来源：http://qqy.smart0.xyz

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://jvg.yuxming.cn

[Q86] 读取 JSON 字段
来源：http://zqa.yuxming.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ltb.zhixingplan.top

[Q87] JSON 字段做条件
来源：http://fzj.yj20258888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iyd.zhengqikj.top

[Q88] 行转列（条件聚合）
来源：http://uep.daxiang520.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hin.zhongyouzk.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://zht.mhx1999.top

[Q89] 判断表是否存在
来源：http://wam.jinghuilouyu.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://ohx.c1oappe.top

[Q90] 生成序号列
来源：http://lul.zhixingplan.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hxe.pengpengdd.cyou

================================================================================
来源：http://woy.tian-w.cn

R. Bash 专题
来源：http://upq.gotoacloud.top

================================================================================
来源：http://zdr.hnxiangtu.top

[R01] shebang 与严格模式
来源：http://jyq.snrcjt.cn

#!/usr/bin/env bash
来源：http://agx.zhiwuduotai.top

set -euo pipefail
来源：http://hmb.316326.xyz

[R02] 变量赋值与使用
来源：http://gca.gogol.net.cn

name="Tom"; echo "$name"
来源：http://bop.bjfxy.top

[R03] 只读变量
来源：http://axp.xinyue.icu

readonly PI=3.14
来源：http://oye.jianghu66.top

[R04] 位置参数
来源：http://buw.ppjwa.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ruh.shanyushiyangtech.top

[R05] 参数默认值
来源：http://zrc.smart0.xyz

name="${1:-default}"
来源：http://gao.hammf.cn

[R06] 判断命令是否存在
来源：http://dzh.guannengcc.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iwe.yanxiufei.cn

[R07] if 判断文件
来源：http://gyz.jqgfzy.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://syh.jinqigfzy.top

[R08] 数值比较
来源：http://aaa.feifeiyinyue.top

if (( a > b )); then echo "a 更大"; fi
来源：http://djp.havefunace.top

[R09] 字符串比较
来源：http://inq.feifeiyinyue.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://doe.hfpthk.cn

[R10] 正则匹配
来源：http://qop.yongpay.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cay.xziqi.cn

[R11] case 多分支
来源：http://fbz.shanyushiyangkeji.top

case "$1" in
来源：http://xmh.nanxinkj.top

start) echo "启动" ;;
来源：http://cvs.jiagoushi.top

stop)  echo "停止" ;;
来源：http://alz.yj20258.top

*)     echo "未知命令" ;;
来源：http://kht.hnqzz.top

esac
来源：http://xom.xylfe.cn

[R12] for 遍历文件
来源：http://ruy.shuidangran.top

for f in *.txt; do echo "$f"; done
来源：http://njf.zhongyouzk.top

[R13] for 计数循环
来源：http://mrb.cqqwz.cn

for i in {1..10}; do echo "$i"; done
来源：http://pix.jinghuilouyu.cn

[R14] C 风格 for
来源：http://hrc.dashuyun.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fhf.ywan-chungtsiang.top

[R15] while 逐行读文件
来源：http://udf.dianchejie.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://sja.ctjpmb.com

[R16] until 等待条件
来源：http://oea.yfazqb.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://pvq.shangyingyoupin.top

[R17] 数组定义与取值
来源：http://ewb.shangyingyoupin.top

arr=(a b c); echo "${arr[0]}"
来源：http://nui.ydzc1.top

[R18] 遍历数组
来源：http://ujf.yfazqb.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ubs.ppjwa.cn

[R19] 数组长度
来源：http://imq.fehbvm.com

echo "${#arr[@]}"
来源：http://jzu.wangdashe.top

[R20] 关联数组（字典）
来源：http://rml.ppjwa.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://yxm.tianlin.xyz

[R21] 字符串长度
来源：http://gbd.jianghu66.top

echo "${#s}"
来源：http://mhp.tianlin.xyz

[R22] 截取子串
来源：http://zya.iojbl.cn

echo "${s:0:5}"
来源：http://ore.jyoumei.cn

[R23] 字符串替换
来源：http://oob.yonumen.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dhm.fktsv.cn

[R24] 大小写转换
来源：http://esr.havefunace.top

echo "${s^^}"; echo "${s,,}"
来源：http://vns.zycfv.cn

[R25] 去后缀 / 去前缀
来源：http://huc.guowangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zlq.birdmap.top

[R26] 命令替换
来源：http://mvh.shangyingyoupin.top

now=$(date +%F); echo "$now"
来源：http://fcg.hammf.cn

[R27] 算术展开
来源：http://cgv.zhijiandao.cn

echo $((1 + 2 * 3))
来源：http://bju.hnqzz.top

[R28] 浮点运算
来源：http://gsr.zycfv.cn

echo "scale=2; 10/3" | bc
来源：http://mjr.uphjek.com

[R29] 定义函数
来源：http://sew.quarkkingdee.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bki.bjfxy.top

[R30] 函数返回状态码
来源：http://pgb.yj20258888.top

f() { return 0; }; f || echo "失败了"
来源：http://xuk.cheryme.top

[R31] 局部变量
来源：http://mhf.jinqigfzy.top

f() { local x=1; echo "$x"; }
来源：http://lam.xziqi.cn

[R32] 参数个数校验
来源：http://lql.zhiwuduotai.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ryp.yuxming.cn

[R33] 捕获错误并提示行号
来源：http://uop.gaohongyu789.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://glj.xingfuxueyuan.xyz

[R34] 退出时清理
来源：http://czi.andypj.xyz

trap 'rm -f "$tmp"' EXIT
来源：http://cnx.daria6918.cn

[R35] 后台执行并等待
来源：http://nrp.haohaochexian.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ipn.gogol.net.cn

[R36] 并发执行多个任务
来源：http://tga.pengpengdd.cyou

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://ipv.zhiwuduotai.top

[R37] 把输出赋给变量
来源：http://fcd.andypj.xyz

files=$(ls -1)
来源：http://qsf.wangdashe.top

[R38] 管道串联
来源：http://spc.ppjwa.cn

cat a.txt | grep -i error | wc -l
来源：http://vhl.sysykeji.top

[R39] 重定向标准输出与错误
来源：http://hcq.tian-w.cn

cmd > out.log 2>&1
来源：http://cgk.cdnleiting.top

[R40] 追加写日志
来源：http://vpc.nanxuanxn.top

echo "log" >> out.log
来源：http://vzf.hesvh.cn

[R41] 丢弃输出
来源：http://ggy.hesvh.cn

cmd >/dev/null 2>&1
来源：http://noy.guowangkeji.top

[R42] 输入重定向
来源：http://kgl.shzxlz.cn

wc -l < a.txt
来源：http://lnx.fzhhl.top

[R43] 按名字查找文件
来源：http://xaj.yvedp.cn

find . -name "*.log" -type f
来源：http://ctk.chenlongwang.top

[R44] 按修改时间查找
来源：http://yau.xuetiantiany.cn

find . -mtime -7 -type f
来源：http://lzz.jqgfzy.top

[R45] 批量删除
来源：http://dhd.feifeiyinyue.top

find . -name "*.tmp" -delete
来源：http://mge.guannengcc.top

[R46] 递归替换文件内容
来源：http://epy.gogol.net.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fkf.sufxvd.cn

[R47] sed 单行替换
来源：http://uis.sufxvd.cn

sed -i 's/foo/bar/g' a.txt
来源：http://jud.tanke756.top

[R48] awk 取指定列
来源：http://ybk.tarul.cn

awk '{print $1, $3}' a.txt
来源：http://xnh.zhengqikj.top

[R49] awk 带条件
来源：http://yzn.9152youxi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kze.zdbjq.cn

[R50] awk 求和
来源：http://zuj.aizwys.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ewa.yanxiufei.cn

[R51] 排序去重取前几
来源：http://swa.yueranfly.top

sort a.txt | uniq -c | sort -rn | head
来源：http://prf.meibo888.top

[R52] 统计行数
来源：http://eop.snrcjt.cn

wc -l a.txt
来源：http://ihu.yongpay.top

[R53] 查看文件头与实时尾
来源：http://hmp.ywan-chungtsiang.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jln.xziqi.cn

[R54] 比较两个文件
来源：http://kel.hysaishi.cn

diff a.txt b.txt
来源：http://qwc.zhiwuduotai.top

[R55] 压缩与解压
来源：http://vsx.zhengqikj.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zjx.kuanghao11.cn

[R56] 远程拷贝
来源：http://oai.dashuyun.cn

scp file user@host:/path/
来源：http://mqj.epnwcf.com

[R57] 远程执行命令
来源：http://zit.0kj1m.cn

ssh user@host 'uptime'
来源：http://jmv.zhongyouzk.top

[R58] 下载文件
来源：http://osf.xuanzx.com

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kng.shangyingyoupin.top

[R59] 发 POST JSON
来源：http://gpz.jiagoushi.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dqq.yueranfly.top

[R60] 只看 HTTP 状态码
来源：http://gli.pengpengdd.cyou

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://whc.jqgufenzy.top

[R61] 磁盘占用
来源：http://jye.daria6918.cn

df -h;  du -sh *
来源：http://ljs.hammf.cn

[R62] 找最占空间的文件
来源：http://jko.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://inl.daxiang520.top

[R63] 内存与进程
来源：http://nvv.gotoacloud.top

free -h;  ps aux | grep nginx
来源：http://iaa.smart0.xyz

[R64] 结束进程
来源：http://ipf.mhx1999.top

kill -9 $(pgrep -f app.py)
来源：http://sfp.wangdashe.top

[R65] 查看端口占用
来源：http://kmx.feifeiyinyue.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://yze.bbcook.cn

[R66] 定时任务
来源：http://psl.iojbl.cn

crontab -e;  crontab -l
来源：http://mkc.xinyue.icu

[R67] 生成随机十六进制串
来源：http://xij.shanyushiyangkeji.top

openssl rand -hex 16
来源：http://uia.hongshengwenyu.top

[R68] 计算文件校验值
来源：http://bty.tian-w.cn

sha256sum a.txt;  md5sum a.txt
来源：http://imx.zhoulong.xyz

[R69] 生成随机密码
来源：http://ixk.jianghu66.top

head -c 16 /dev/urandom | base64
来源：http://rze.dianchejie.cn

[R70] 时间戳与互转
来源：http://spx.nanxuanxn.top

date +%s;  date -d @1700000000
来源：http://qte.cucudq.cn

[R71] 日期格式化
来源：http://jds.zycfv.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ibq.shanyushiyangkeji.top

[R72] 等待端口就绪
来源：http://xvo.shzxlz.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cew.mhx1999.top

[R73] 分割大日志
来源：http://fiu.hnqzz.top

split -l 1000 big.log part_
来源：http://osf.aizwys.cn

[R74] 批量重命名
来源：http://agv.nanxinkj.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wds.gzhubu.top

[R75] 导出环境变量
来源：http://rtj.xuanzx.com

export PATH="$HOME/bin:$PATH"
来源：http://jwo.xylfe.cn

[R76] 使用临时文件
来源：http://meu.fktsv.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zzs.guannengcc.top

[R77] 读取用户输入
来源：http://efw.ppjwa.cn

read -rp "请输入: " ans
来源：http://cmz.guowangkeji.top

[R78] 交互式菜单
来源：http://qcv.fanxiaobao.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://afo.tanke756.top

[R79] 解析命令行选项
来源：http://sva.tian-w.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oub.dashuyun.cn

[R80] 查看脚本执行耗时
来源：http://cpv.vqdsnc.cn

time ./run.sh
来源：http://owc.jyoumei.cn

================================================================================
来源：http://qxe.xinyue.icu

S. C / C++ 专题
来源：http://ied.sufxvd.cn

================================================================================
来源：http://rei.wangdashe.top

[S01] C：Hello World
来源：http://gxv.gzhubu.top

#include <stdio.h>
来源：http://sey.bbcook.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xrf.ctjpmb.com

[S02] C：变量与格式化输出
来源：http://bbd.jyoumei.cn

int a = 10; printf("%d\n", a);
来源：http://cqj.havefunace.top

[S03] C：读入整数
来源：http://gus.0kj1m.cn

int x; scanf("%d", &x);
来源：http://pdn.hcnkem.com

[S04] C：字符串复制
来源：http://btb.jinqigfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://miz.daria6918.cn

[S05] C：字符串长度
来源：http://sgj.hongshengwenyu.top

strlen(s)
来源：http://jsj.yj20258888.top

[S06] C：字符串比较
来源：http://xiq.ehwqpu.com

strcmp(a, b) == 0
来源：http://ezy.sweek.top

[S07] C：数组遍历求和
来源：http://gxu.wangdashe.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ddd.ppjwa.cn

[S08] C：动态内存分配与释放
来源：http://mxa.zhengqikj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fcg.yj20258.top

[S09] C：结构体定义与初始化
来源：http://ycw.jinqigufen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cbk.meibo888.top

[S10] C：指针与解引用
来源：http://dfh.iojbl.cn

int *p = &a;  *p = 5;
来源：http://ubr.snrcjt.cn

[S11] C：逐行读文件
来源：http://zsq.hesvh.cn

FILE *f = fopen("a.txt", "r");
来源：http://zcn.ppjwa.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xpq.ppjwa.cn

fclose(f);
来源：http://bfz.jlsjyb.cn

[S12] C：写文件
来源：http://gab.shuidangran.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sgg.hammf.cn

[S13] C：宏定义
来源：http://xpe.feifeiyinyue.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mkb.chenzaomai.com

[S14] C：枚举
来源：http://osx.zhongyouzk.top

enum Color { RED, GREEN, BLUE };
来源：http://dnm.gzhubu.top

[S15] C：类型转换
来源：http://wny.zhixingplan.top

(double) a / b
来源：http://der.shangyingyoupin.top

[S16] C：位操作置位
来源：http://mnr.jqgfzy.top

x |= (1 << 3);
来源：http://tws.hammf.cn

[S17] C：安全拼接字符串
来源：http://let.shanyushiyangkeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jia.tian-w.cn

[S18] C：命令行参数
来源：http://qtn.sysykeji.top

int main(int argc, char **argv)
来源：http://hqe.ivvv.top

[S19] C：快速排序
来源：http://kii.sxryk.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qnp.yueranfly.top

[S20] C：二分查找
来源：http://cky.fanxiaobao.xyz


<!-- 参考信息 -->