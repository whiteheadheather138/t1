代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://usd.jinqigfzy.top

[Q50] 批量更新
来源：http://ecx.daria6918.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://akm.nanxuanxn.top

[Q51] 用子查询更新
来源：http://mfu.sjlbkw.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://smh.sysykeji.top

[Q52] 删除指定行
来源：http://fxw.shzxlz.cn

DELETE FROM users WHERE id = 10;
来源：http://dfq.sysykeji.top

[Q53] 按条件删除
来源：http://vuo.svipenyu.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uqt.yvedp.cn

[Q54] 清空表
来源：http://zrp.nanxinkj.top

TRUNCATE TABLE logs;
来源：http://nbq.ehwqpu.com

[Q55] 排名（并列占位）
来源：http://jeb.fanxiaobao.xyz

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wcf.sufxvd.cn

[Q56] 密集排名（并列不占位）
来源：http://esy.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://uxp.9152youxi.cn

[Q57] 行号
来源：http://yii.fktsv.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://dys.fzhhl.top

[Q58] 累计求和
来源：http://sfv.hysaishi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pos.cucudq.cn

[Q59] 分组内累计
来源：http://nzc.c1oappe.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://isb.feifeiyinyue.top

[Q60] 取上一行 / 下一行
来源：http://wvr.gogol.net.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://owm.yueranfly.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://nlz.fzhhl.top

[Q61] 移动平均
来源：http://qbu.wangshuangyany.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://max.epnwcf.com

[Q62] 分组占比
来源：http://rsr.daxiang520.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xuw.316326.xyz

[Q63] 开启事务
来源：http://klh.wangshuangyany.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://gne.0kj1m.cn

[Q64] 提交事务
来源：http://can.cheryme.top

COMMIT;
来源：http://iah.gaohongyu789.top

[Q65] 回滚事务
来源：http://wkc.shanyushiyangtech.top

ROLLBACK;
来源：http://afv.zdqjudy.top

[Q66] 行锁查询
来源：http://ugu.cdnleiting.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bpb.yanxiufei.cn

[Q67] 设置隔离级别
来源：http://bsz.cqqwz.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://phh.ivvv.top

[Q68] 保存点
来源：http://xvj.gotoacloud.top

SAVEPOINT sp1;
来源：http://mzt.fzhhl.top

ROLLBACK TO sp1;
来源：http://rnb.xinyue.icu

[Q69] 查看执行计划
来源：http://pyd.yuanzhike.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vsl.xuanzx.com

[Q70] 更新统计信息
来源：http://bue.zhengqikj.top

ANALYZE TABLE users;
来源：http://bpt.zhaomingkeji.xyz

[Q71] 查看建表语句
来源：http://ftn.cqqwz.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qdw.yj202588.top

[Q72] 查看索引
来源：http://zjg.xuetiantiany.cn

SHOW INDEX FROM users;
来源：http://vim.guannengcc.top

[Q73] 查看表状态
来源：http://nfc.yuxming.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://kev.zhaomingkeji.xyz

[Q74] 强制使用索引
来源：http://qbl.hnxiangtu.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ubw.zhiwuduotai.top

[Q75] 日期格式化
来源：http://gpc.tian-w.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://tru.yfazqb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://rqk.xylfe.cn

[Q76] 按天统计
来源：http://afr.yj20258.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hho.chenlongwang.top

[Q77] 时间加减
来源：http://umx.daxiang520.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uiz.tarul.cn

[Q78] 当前时间
来源：http://efv.shanyushiyangkeji.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qqc.sufxvd.cn

[Q79] 字符串拼接
来源：http://ptg.jinqigufen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bab.hcnkem.com

[Q80] 字符串截取
来源：http://unc.gzhubu.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://agr.snrcjt.cn

[Q81] 字符串替换
来源：http://gkh.chenlongwang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://khs.ehwqpu.com

[Q82] 字符长度与字节长度
来源：http://skd.fzhhl.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://dju.feifeiyinyue.top

[Q83] 大小写转换
来源：http://trv.jyoumei.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kjw.9152youxi.cn

[Q84] 去除首尾空格
来源：http://wsp.wangdashe.top

SELECT TRIM(name) FROM users;
来源：http://tzb.guannengcc.top

[Q85] 数值取整
来源：http://ado.fengsongda.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://lud.shanyushiyangtech.top

[Q86] 读取 JSON 字段
来源：http://iyj.sxryk.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pmg.hnxiangtu.top

[Q87] JSON 字段做条件
来源：http://wfs.xinyue.icu

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jyn.sufxvd.cn

[Q88] 行转列（条件聚合）
来源：http://nrz.yanxiufei.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://iml.yj202588.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ver.svipenyu.cn

[Q89] 判断表是否存在
来源：http://vrm.bjfxy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://gda.tarul.cn

[Q90] 生成序号列
来源：http://dbk.jlsjyb.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://tog.shangyingyoupin.top

================================================================================
来源：http://wjo.hysaishi.cn

R. Bash 专题
来源：http://rqs.pengpengdd.cyou

================================================================================
来源：http://iix.hnxiangtu.top

[R01] shebang 与严格模式
来源：http://mkn.zhiwuduotai.top

#!/usr/bin/env bash
来源：http://rzo.xuanzx.com

set -euo pipefail
来源：http://wzt.gzhubu.top

[R02] 变量赋值与使用
来源：http://ywl.mhx1999.top

name="Tom"; echo "$name"
来源：http://kzp.aibaodan.cn

[R03] 只读变量
来源：http://ytr.vqdsnc.cn

readonly PI=3.14
来源：http://jsh.aizwys.cn

[R04] 位置参数
来源：http://bnk.tian-w.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://nng.xuanzx.com

[R05] 参数默认值
来源：http://kuv.pengpengdd.cyou

name="${1:-default}"
来源：http://pdg.fanxiaobao.xyz

[R06] 判断命令是否存在
来源：http://uod.kuanghao11.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yhn.jinghuilouyu.cn

[R07] if 判断文件
来源：http://ykr.uphjek.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vjg.kuanghao11.cn

[R08] 数值比较
来源：http://ext.mhx1999.top

if (( a > b )); then echo "a 更大"; fi
来源：http://hep.xuetiantiany.cn

[R09] 字符串比较
来源：http://esy.iojbl.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://ylg.dianchejie.cn

[R10] 正则匹配
来源：http://trk.nanxinkj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xek.0kj1m.cn

[R11] case 多分支
来源：http://bcy.shangyingyoupin.top

case "$1" in
来源：http://gcq.zhixingplan.top

start) echo "启动" ;;
来源：http://plh.hesvh.cn

stop)  echo "停止" ;;
来源：http://jkp.jlsjyb.cn

*)     echo "未知命令" ;;
来源：http://car.tanke756.top

esac
来源：http://xvd.chenlongwang.top

[R12] for 遍历文件
来源：http://xpj.tanke756.top

for f in *.txt; do echo "$f"; done
来源：http://brh.ybcxt.top

[R13] for 计数循环
来源：http://qcd.jqgufenzy.top

for i in {1..10}; do echo "$i"; done
来源：http://vqm.gaohongyu789.top

[R14] C 风格 for
来源：http://bis.hysaishi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://bdo.pycfn.com

[R15] while 逐行读文件
来源：http://htl.jinyuanbaomall.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://zyq.hesvh.cn

[R16] until 等待条件
来源：http://ndw.tanke756.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://igp.yangfankeji.com

[R17] 数组定义与取值
来源：http://fts.hysaishi.cn

arr=(a b c); echo "${arr[0]}"
来源：http://mrl.mhx1999.top

[R18] 遍历数组
来源：http://xho.zycfv.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://pfe.yj20258.top

[R19] 数组长度
来源：http://vmi.yonumen.top

echo "${#arr[@]}"
来源：http://drq.ybcxt.top

[R20] 关联数组（字典）
来源：http://yum.aibaodan.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zyw.fktsv.cn

[R21] 字符串长度
来源：http://nlc.tarul.cn

echo "${#s}"
来源：http://msu.shanyushiyangtech.top

[R22] 截取子串
来源：http://sqk.cashguo.top

echo "${s:0:5}"
来源：http://hyd.yonumen.top

[R23] 字符串替换
来源：http://kly.yj202588.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jwf.chenjidiqi.icu

[R24] 大小写转换
来源：http://bbc.shanyushiyangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://ecz.jyoumei.cn

[R25] 去后缀 / 去前缀
来源：http://guw.meibo888.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://zan.jinghuilouyu.cn

[R26] 命令替换
来源：http://qrr.gzhubu.top

now=$(date +%F); echo "$now"
来源：http://hrc.hywenlv.cn

[R27] 算术展开
来源：http://wnh.vehdjk.com

echo $((1 + 2 * 3))
来源：http://qxa.andypj.xyz

[R28] 浮点运算
来源：http://hvd.kuanghao11.cn

echo "scale=2; 10/3" | bc
来源：http://sus.sufxvd.cn

[R29] 定义函数
来源：http://lwu.ywan-chungtsiang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://pme.ctjpmb.com

[R30] 函数返回状态码
来源：http://tys.redwolf501.top

f() { return 0; }; f || echo "失败了"
来源：http://yls.tarul.cn

[R31] 局部变量
来源：http://xel.pycfn.com

f() { local x=1; echo "$x"; }
来源：http://usu.hongshengwenyu.top

[R32] 参数个数校验
来源：http://ekc.hywenlv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ioj.yj202588.top

[R33] 捕获错误并提示行号
来源：http://dqv.feifeiyinyue.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ubn.xinyue.icu

[R34] 退出时清理
来源：http://tzg.jyoumei.cn

trap 'rm -f "$tmp"' EXIT
来源：http://jss.nanxinkj.top

[R35] 后台执行并等待
来源：http://rsu.yonumen.top

sleep 5 & pid=$!; wait "$pid"
来源：http://kvi.snrcjt.cn

[R36] 并发执行多个任务
来源：http://ltj.tanke756.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://skj.shanyushiyangtech.top

[R37] 把输出赋给变量
来源：http://mhh.0kj1m.cn

files=$(ls -1)
来源：http://zfh.yonumen.top

[R38] 管道串联
来源：http://yax.ybcxt.top

cat a.txt | grep -i error | wc -l
来源：http://bsl.ppjwa.cn

[R39] 重定向标准输出与错误
来源：http://sgb.zdqjudy.top

cmd > out.log 2>&1
来源：http://umt.hysaishi.cn

[R40] 追加写日志
来源：http://kxv.ppjwa.cn

echo "log" >> out.log
来源：http://pvr.sysykeji.top

[R41] 丢弃输出
来源：http://nwm.guowangkeji.top

cmd >/dev/null 2>&1
来源：http://lqv.aibaodan.cn

[R42] 输入重定向
来源：http://ebm.xingfuxueyuan.xyz

wc -l < a.txt
来源：http://vdu.chenjidiqi.icu

[R43] 按名字查找文件
来源：http://cuj.ydzc1.top

find . -name "*.log" -type f
来源：http://yxg.jianghu66.top

[R44] 按修改时间查找
来源：http://nav.meibo888.top

find . -mtime -7 -type f
来源：http://lum.ehwqpu.com

[R45] 批量删除
来源：http://rmn.jinqigfzy.top

find . -name "*.tmp" -delete
来源：http://zia.redwolf501.top

[R46] 递归替换文件内容
来源：http://are.0kj1m.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kzx.gzhubu.top

[R47] sed 单行替换
来源：http://oes.316326.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://ixt.birdmap.top

[R48] awk 取指定列
来源：http://qpi.zhijiandao.cn

awk '{print $1, $3}' a.txt
来源：http://frw.zhiwuduotai.top

[R49] awk 带条件
来源：http://vii.yfazqb.com

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://szl.iojbl.cn

[R50] awk 求和
来源：http://btm.shuidangran.top

awk '{s += $2} END {print s}' a.txt
来源：http://oeg.kuanghao11.cn

[R51] 排序去重取前几
来源：http://jec.zhengqikj.top

sort a.txt | uniq -c | sort -rn | head
来源：http://prc.nanxinkj.top

[R52] 统计行数
来源：http://dkr.hywenlv.cn

wc -l a.txt
来源：http://bfo.0kj1m.cn

[R53] 查看文件头与实时尾
来源：http://xog.sxryk.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://efk.yj20258.top

[R54] 比较两个文件
来源：http://ksu.nanxinkj.top

diff a.txt b.txt
来源：http://lcd.vqdsnc.cn

[R55] 压缩与解压
来源：http://xfj.sxryk.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kij.yvedp.cn

[R56] 远程拷贝
来源：http://wuz.hesvh.cn

scp file user@host:/path/
来源：http://gqm.shangyingyoupin.top

[R57] 远程执行命令
来源：http://zmi.hongshengwenyu.top

ssh user@host 'uptime'
来源：http://anr.hnqzz.top

[R58] 下载文件
来源：http://oks.jqgufenzy.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yrz.gogol.net.cn

[R59] 发 POST JSON
来源：http://upt.feifeiyinyue.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://roo.ppjwa.cn

[R60] 只看 HTTP 状态码
来源：http://uds.hongshengwenyu.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dgp.aizwys.cn

[R61] 磁盘占用
来源：http://ise.yueranfly.top

df -h;  du -sh *
来源：http://uts.yj20258.top

[R62] 找最占空间的文件
来源：http://lcq.tian-w.cn

du -ah . | sort -rh | head -10
来源：http://xax.sufxvd.cn

[R63] 内存与进程
来源：http://shp.yonumen.top

free -h;  ps aux | grep nginx
来源：http://iiw.wangdashe.top

[R64] 结束进程
来源：http://pvi.zhiwuduotai.top

kill -9 $(pgrep -f app.py)
来源：http://mxr.shzxlz.cn

[R65] 查看端口占用
来源：http://wgb.ybcxt.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jzh.shuidangran.top

[R66] 定时任务
来源：http://xho.pengpengdd.cyou

crontab -e;  crontab -l
来源：http://tty.shanyushiyangtech.top

[R67] 生成随机十六进制串
来源：http://aca.yanxiufei.cn

openssl rand -hex 16
来源：http://fgj.shangyingyoupin.top

[R68] 计算文件校验值
来源：http://vga.cheryme.top

sha256sum a.txt;  md5sum a.txt
来源：http://gos.cqqwz.cn

[R69] 生成随机密码
来源：http://rps.hnxiangtu.top

head -c 16 /dev/urandom | base64
来源：http://usw.cdnleiting.top

[R70] 时间戳与互转
来源：http://gcp.shuidangran.top

date +%s;  date -d @1700000000
来源：http://osd.nwbrower.top

[R71] 日期格式化
来源：http://eym.gotoacloud.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://vfz.yvedp.cn

[R72] 等待端口就绪
来源：http://eho.fanxiaobao.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://kyy.xziqi.cn

[R73] 分割大日志
来源：http://cxf.9152youxi.cn

split -l 1000 big.log part_
来源：http://ehq.shanyushiyangtech.top

[R74] 批量重命名
来源：http://abc.jinyuanbaomall.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://lal.yuanzhike.top

[R75] 导出环境变量
来源：http://msq.yj202588.top

export PATH="$HOME/bin:$PATH"
来源：http://ozy.cqqwz.cn

[R76] 使用临时文件
来源：http://zex.gotoacloud.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://inz.sufxvd.cn

[R77] 读取用户输入
来源：http://kzu.yongpay.top

read -rp "请输入: " ans
来源：http://sqd.zhiwuduotai.top

[R78] 交互式菜单
来源：http://rnd.zdqjudy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://evt.yanxiufei.cn

[R79] 解析命令行选项
来源：http://xau.hfpthk.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://srm.chenjidiqi.icu

[R80] 查看脚本执行耗时
来源：http://vom.jiagoushi.top

time ./run.sh
来源：http://fjw.cdnleiting.top

================================================================================
来源：http://lda.zycfv.cn

S. C / C++ 专题
来源：http://osl.9152youxi.cn

================================================================================
来源：http://pqz.yueranfly.top

[S01] C：Hello World
来源：http://ctt.redwolf501.top

#include <stdio.h>
来源：http://mbq.sysykeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wxp.daxiang520.top

[S02] C：变量与格式化输出
来源：http://rmg.wangshuangyany.cn

int a = 10; printf("%d\n", a);
来源：http://cqs.sweek.top

[S03] C：读入整数
来源：http://ure.andypj.xyz

int x; scanf("%d", &x);
来源：http://kyg.52xcode.cn

[S04] C：字符串复制
来源：http://sqk.fehbvm.com

char dst[32]; strcpy(dst, "hi");
来源：http://szl.sxryk.cn

[S05] C：字符串长度
来源：http://rxi.dianchejie.cn

strlen(s)
来源：http://ixb.fzhhl.top

[S06] C：字符串比较
来源：http://lkw.0kj1m.cn

strcmp(a, b) == 0
来源：http://qtv.uphjek.com

[S07] C：数组遍历求和
来源：http://iwh.zhengqikj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://exy.hammf.cn

[S08] C：动态内存分配与释放
来源：http://uqh.zhengqikj.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ncd.chenjidiqi.icu

[S09] C：结构体定义与初始化
来源：http://unt.cheryme.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://yjj.hongshengwenyu.top

[S10] C：指针与解引用
来源：http://udp.zhaomingkeji.xyz

int *p = &a;  *p = 5;
来源：http://pyu.pengpengdd.cyou

[S11] C：逐行读文件
来源：http://ibt.316326.xyz

FILE *f = fopen("a.txt", "r");
来源：http://nvl.jlsjyb.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sbn.zdqjudy.top

fclose(f);
来源：http://btc.smart0.xyz

[S12] C：写文件
来源：http://bce.jqgfzy.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xhx.aibaodan.cn

[S13] C：宏定义
来源：http://mxm.0kj1m.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://tjc.gogol.net.cn

[S14] C：枚举
来源：http://fjr.bjfxy.top

enum Color { RED, GREEN, BLUE };
来源：http://roq.yueranfly.top

[S15] C：类型转换
来源：http://qfs.yanxiufei.cn

(double) a / b
来源：http://qzt.gzhubu.top

[S16] C：位操作置位
来源：http://laq.zhijiandao.cn

x |= (1 << 3);
来源：http://pjd.xylfe.cn

[S17] C：安全拼接字符串
来源：http://npk.jinqigufen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jjg.vqdsnc.cn

[S18] C：命令行参数
来源：http://anw.andypj.xyz

int main(int argc, char **argv)
来源：http://iha.smart0.xyz

[S19] C：快速排序
来源：http://smh.svipenyu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://doa.wangdashe.top

[S20] C：二分查找
来源：http://afi.jyoumei.cn


<!-- 参考信息 -->