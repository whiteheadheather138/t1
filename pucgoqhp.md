代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://oai.yuanzhike.top

[Q52] 删除指定行
来源：http://bqv.9152youxi.cn

DELETE FROM users WHERE id = 10;
来源：http://kbd.xingfuxueyuan.xyz

[Q53] 按条件删除
来源：http://nez.birdmap.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://iwy.fzhhl.top

[Q54] 清空表
来源：http://bkk.yj20258.top

TRUNCATE TABLE logs;
来源：http://iqf.ydzc1.top

[Q55] 排名（并列占位）
来源：http://ohg.yfazqb.com

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://exg.xziqi.cn

[Q56] 密集排名（并列不占位）
来源：http://zaf.zhijiandao.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://xdr.xingfuxueyuan.xyz

[Q57] 行号
来源：http://xfy.yongpay.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cti.sweek.top

[Q58] 累计求和
来源：http://gjz.jqgfzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://oqi.fzhhl.top

[Q59] 分组内累计
来源：http://fva.birdmap.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hqp.shuidangran.top

[Q60] 取上一行 / 下一行
来源：http://xxl.cheryme.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yah.sweek.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://cmg.tian-w.cn

[Q61] 移动平均
来源：http://xcb.jinyuanbaomall.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://aqq.316326.xyz

[Q62] 分组占比
来源：http://onz.sjlbkw.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://aew.tian-w.cn

[Q63] 开启事务
来源：http://oyw.aibaodan.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://pzt.xuanzx.com

[Q64] 提交事务
来源：http://kab.hnxiangtu.top

COMMIT;
来源：http://kmq.jyoumei.cn

[Q65] 回滚事务
来源：http://nun.epnwcf.com

ROLLBACK;
来源：http://jjk.yvedp.cn

[Q66] 行锁查询
来源：http://zfh.birdmap.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eyx.jianghu66.top

[Q67] 设置隔离级别
来源：http://fpf.shanyushiyangkeji.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://sol.jqgfzy.top

[Q68] 保存点
来源：http://cbn.sysykeji.top

SAVEPOINT sp1;
来源：http://kyn.svipenyu.cn

ROLLBACK TO sp1;
来源：http://gls.jinyuanbaomall.cn

[Q69] 查看执行计划
来源：http://cip.hnxiangtu.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://fon.hongshengwenyu.top

[Q70] 更新统计信息
来源：http://yez.havefunace.top

ANALYZE TABLE users;
来源：http://hsk.quarkkingdee.top

[Q71] 查看建表语句
来源：http://ozd.yj20258.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://axi.redwolf501.top

[Q72] 查看索引
来源：http://usc.sweek.top

SHOW INDEX FROM users;
来源：http://zuz.ppjwa.cn

[Q73] 查看表状态
来源：http://oki.jinyuanbaomall.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://yvt.ywan-chungtsiang.top

[Q74] 强制使用索引
来源：http://mzs.xziqi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://bih.ehwqpu.com

[Q75] 日期格式化
来源：http://lro.dashuyun.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://arv.haohaochexian.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qns.jinyuanbaomall.cn

[Q76] 按天统计
来源：http://xrr.vehdjk.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://spm.xinyue.icu

[Q77] 时间加减
来源：http://ers.ydzc1.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wzl.pengpengdd.cyou

[Q78] 当前时间
来源：http://czv.ydzc1.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ojv.hfpthk.cn

[Q79] 字符串拼接
来源：http://nsj.snrcjt.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hgz.jinqigfzy.top

[Q80] 字符串截取
来源：http://nhy.iojbl.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kzu.ydjk.org.cn

[Q81] 字符串替换
来源：http://hcv.sweek.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://pdu.ydjk.org.cn

[Q82] 字符长度与字节长度
来源：http://bzp.cashguo.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sxz.jinyuanbaomall.cn

[Q83] 大小写转换
来源：http://ovj.xziqi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hay.fanxiaobao.xyz

[Q84] 去除首尾空格
来源：http://hsj.yj202588.top

SELECT TRIM(name) FROM users;
来源：http://drl.yangfankeji.com

[Q85] 数值取整
来源：http://gck.tian-w.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://srr.daria6918.cn

[Q86] 读取 JSON 字段
来源：http://dzx.xylfe.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://olw.ctjpmb.com

[Q87] JSON 字段做条件
来源：http://kqf.shuidangran.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rrt.hammf.cn

[Q88] 行转列（条件聚合）
来源：http://juc.jinghuilouyu.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fet.vehdjk.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://pio.yj20258.top

[Q89] 判断表是否存在
来源：http://ulm.cheryme.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kev.ywan-chungtsiang.top

[Q90] 生成序号列
来源：http://jio.yuxming.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://awe.yanxiufei.cn

================================================================================
来源：http://wsg.yfazqb.com

R. Bash 专题
来源：http://mvn.chenlongwang.top

================================================================================
来源：http://jzt.yonumen.top

[R01] shebang 与严格模式
来源：http://egb.xuanzx.com

#!/usr/bin/env bash
来源：http://xaf.zdqjudy.top

set -euo pipefail
来源：http://rrg.jqgfzy.top

[R02] 变量赋值与使用
来源：http://fuj.zhijiandao.cn

name="Tom"; echo "$name"
来源：http://sbo.fanxiaobao.xyz

[R03] 只读变量
来源：http://lct.daxiang520.top

readonly PI=3.14
来源：http://mfu.cdnleiting.top

[R04] 位置参数
来源：http://rrc.aizwys.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://suv.ivvv.top

[R05] 参数默认值
来源：http://vra.dashuyun.cn

name="${1:-default}"
来源：http://gni.sweek.top

[R06] 判断命令是否存在
来源：http://fut.jyoumei.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://nqx.hesvh.cn

[R07] if 判断文件
来源：http://cdm.ivvv.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://jtw.gogol.net.cn

[R08] 数值比较
来源：http://ljm.xuanzx.com

if (( a > b )); then echo "a 更大"; fi
来源：http://vea.hongshengwenyu.top

[R09] 字符串比较
来源：http://sjl.xinyue.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fgf.jqgfzy.top

[R10] 正则匹配
来源：http://xlb.zhengqikj.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://xpz.xinyue.icu

[R11] case 多分支
来源：http://uwo.zdbjq.cn

case "$1" in
来源：http://vpe.svipenyu.cn

start) echo "启动" ;;
来源：http://kgy.jianghu66.top

stop)  echo "停止" ;;
来源：http://wqy.hcnkem.com

*)     echo "未知命令" ;;
来源：http://viz.dianchejie.cn

esac
来源：http://fki.dianchejie.cn

[R12] for 遍历文件
来源：http://xww.aizwys.cn

for f in *.txt; do echo "$f"; done
来源：http://whr.cashguo.top

[R13] for 计数循环
来源：http://loc.quarkkingdee.top

for i in {1..10}; do echo "$i"; done
来源：http://meb.jinyuanbaomall.cn

[R14] C 风格 for
来源：http://hqs.fengsongda.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://uyo.xuanzx.com

[R15] while 逐行读文件
来源：http://bgp.fengsongda.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vfp.ybcxt.top

[R16] until 等待条件
来源：http://ntj.zhongyouzk.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xql.ctjpmb.com

[R17] 数组定义与取值
来源：http://tmj.ydjk.org.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kmc.fengsongda.top

[R18] 遍历数组
来源：http://azn.hesvh.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://emb.cqqwz.cn

[R19] 数组长度
来源：http://hrs.hammf.cn

echo "${#arr[@]}"
来源：http://xqt.cheryme.top

[R20] 关联数组（字典）
来源：http://vxq.zdbjq.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ibh.cucudq.cn

[R21] 字符串长度
来源：http://xlj.fanxiaobao.xyz

echo "${#s}"
来源：http://uzv.andypj.xyz

[R22] 截取子串
来源：http://nrk.yueranfly.top

echo "${s:0:5}"
来源：http://aoz.daxiang520.top

[R23] 字符串替换
来源：http://djc.shangyingyoupin.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://iut.birdmap.top

[R24] 大小写转换
来源：http://qfo.zhixingplan.top

echo "${s^^}"; echo "${s,,}"
来源：http://vcd.shanyushiyangtech.top

[R25] 去后缀 / 去前缀
来源：http://ahu.yuanzhike.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mfm.sufxvd.cn

[R26] 命令替换
来源：http://qei.yonumen.top

now=$(date +%F); echo "$now"
来源：http://yjl.sysykeji.top

[R27] 算术展开
来源：http://cew.feifeiyinyue.top

echo $((1 + 2 * 3))
来源：http://vtx.smart0.xyz

[R28] 浮点运算
来源：http://dha.jinqigfzy.top

echo "scale=2; 10/3" | bc
来源：http://hhw.nanxuanxn.top

[R29] 定义函数
来源：http://wcb.fanxiaobao.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://loc.wangdashe.top

[R30] 函数返回状态码
来源：http://kjb.cheryme.top

f() { return 0; }; f || echo "失败了"
来源：http://zcw.snrcjt.cn

[R31] 局部变量
来源：http://nso.jqgfzy.top

f() { local x=1; echo "$x"; }
来源：http://dap.quarkkingdee.top

[R32] 参数个数校验
来源：http://vzd.shzxlz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://juy.xingfuxueyuan.xyz

[R33] 捕获错误并提示行号
来源：http://mbm.shanyushiyangkeji.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://lwd.chenlongwang.top

[R34] 退出时清理
来源：http://lml.c1oappe.top

trap 'rm -f "$tmp"' EXIT
来源：http://vzw.fehbvm.com

[R35] 后台执行并等待
来源：http://lii.yuanzhike.top

sleep 5 & pid=$!; wait "$pid"
来源：http://icv.haohaochexian.top

[R36] 并发执行多个任务
来源：http://aya.haohaochexian.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nld.ydzc1.top

[R37] 把输出赋给变量
来源：http://vkr.fengsongda.top

files=$(ls -1)
来源：http://yup.yangfankeji.com

[R38] 管道串联
来源：http://uaa.yuxming.cn

cat a.txt | grep -i error | wc -l
来源：http://dva.kuanghao11.cn

[R39] 重定向标准输出与错误
来源：http://pwg.cdnleiting.top

cmd > out.log 2>&1
来源：http://zsx.iojbl.cn

[R40] 追加写日志
来源：http://nzn.zhengqikj.top

echo "log" >> out.log
来源：http://tgo.shangyingyoupin.top

[R41] 丢弃输出
来源：http://meu.tian-w.cn

cmd >/dev/null 2>&1
来源：http://jug.shanyushiyangkeji.top

[R42] 输入重定向
来源：http://bbq.hesvh.cn

wc -l < a.txt
来源：http://ckl.gotoacloud.top

[R43] 按名字查找文件
来源：http://hvw.hesvh.cn

find . -name "*.log" -type f
来源：http://bsr.hfpthk.cn

[R44] 按修改时间查找
来源：http://vfk.hnxiangtu.top

find . -mtime -7 -type f
来源：http://ucd.ppjwa.cn

[R45] 批量删除
来源：http://uoc.guowangkeji.top

find . -name "*.tmp" -delete
来源：http://rai.sjlbkw.cn

[R46] 递归替换文件内容
来源：http://ikw.jianghu66.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://loc.ywan-chungtsiang.top

[R47] sed 单行替换
来源：http://izv.fengsongda.top

sed -i 's/foo/bar/g' a.txt
来源：http://qkg.birdmap.top

[R48] awk 取指定列
来源：http://toa.tian-w.cn

awk '{print $1, $3}' a.txt
来源：http://qke.tian-w.cn

[R49] awk 带条件
来源：http://kiq.aizwys.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://qim.cdnleiting.top

[R50] awk 求和
来源：http://cqc.hysaishi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://rql.nwbrower.top

[R51] 排序去重取前几
来源：http://jvn.zhijiandao.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qhe.jinghuilouyu.cn

[R52] 统计行数
来源：http://brm.hcnkem.com

wc -l a.txt
来源：http://jys.gotoacloud.top

[R53] 查看文件头与实时尾
来源：http://hip.shanyushiyangkeji.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uji.gaohongyu789.top

[R54] 比较两个文件
来源：http://ujv.xziqi.cn

diff a.txt b.txt
来源：http://wzv.yj202588.top

[R55] 压缩与解压
来源：http://pkb.9152youxi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://zjs.sufxvd.cn

[R56] 远程拷贝
来源：http://vdl.yueranfly.top

scp file user@host:/path/
来源：http://lju.sweek.top

[R57] 远程执行命令
来源：http://hps.316326.xyz

ssh user@host 'uptime'
来源：http://nij.jinyuanbaomall.cn

[R58] 下载文件
来源：http://kzw.fengsongda.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jpd.haohaochexian.top

[R59] 发 POST JSON
来源：http://kph.zdbjq.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nfn.fengsongda.top

[R60] 只看 HTTP 状态码
来源：http://org.cheryme.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wzg.jqgufenzy.top

[R61] 磁盘占用
来源：http://lfx.jianghu66.top

df -h;  du -sh *
来源：http://wlh.yanxiufei.cn

[R62] 找最占空间的文件
来源：http://cin.tianlin.xyz

du -ah . | sort -rh | head -10
来源：http://grm.yonumen.top

[R63] 内存与进程
来源：http://pbb.jinyuanbaomall.cn

free -h;  ps aux | grep nginx
来源：http://ygj.cashguo.top

[R64] 结束进程
来源：http://ref.andypj.xyz

kill -9 $(pgrep -f app.py)
来源：http://ntv.ydjk.org.cn

[R65] 查看端口占用
来源：http://tgl.hnxiangtu.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bwj.shzxlz.cn

[R66] 定时任务
来源：http://upc.pycfn.com

crontab -e;  crontab -l
来源：http://zsa.hammf.cn

[R67] 生成随机十六进制串
来源：http://vmq.zdqjudy.top

openssl rand -hex 16
来源：http://pev.hnxiangtu.top

[R68] 计算文件校验值
来源：http://kaw.bbcook.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tod.0kj1m.cn

[R69] 生成随机密码
来源：http://imx.316326.xyz

head -c 16 /dev/urandom | base64
来源：http://ghz.xuetiantiany.cn

[R70] 时间戳与互转
来源：http://aam.mhx1999.top

date +%s;  date -d @1700000000
来源：http://ppg.jqgufenzy.top

[R71] 日期格式化
来源：http://geh.hfpthk.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yfk.iojbl.cn

[R72] 等待端口就绪
来源：http://axz.jyoumei.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://afi.gotoacloud.top

[R73] 分割大日志
来源：http://qwj.shzxlz.cn

split -l 1000 big.log part_
来源：http://mmt.aibaodan.cn

[R74] 批量重命名
来源：http://otd.gaohongyu789.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sqj.52xcode.cn

[R75] 导出环境变量
来源：http://ayo.ydjk.org.cn

export PATH="$HOME/bin:$PATH"
来源：http://ywa.feifeiyinyue.top

[R76] 使用临时文件
来源：http://tin.hysaishi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dqp.vehdjk.com

[R77] 读取用户输入
来源：http://uey.bjfxy.top

read -rp "请输入: " ans
来源：http://txd.chenzaomai.com

[R78] 交互式菜单
来源：http://cxo.yvedp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://pwv.yj20258888.top

[R79] 解析命令行选项
来源：http://iig.zhoulong.xyz

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pcq.jinqigufen.top

[R80] 查看脚本执行耗时
来源：http://cny.jinyuanbaomall.cn

time ./run.sh
来源：http://qqj.hammf.cn

================================================================================
来源：http://bgo.nanxuanxn.top

S. C / C++ 专题
来源：http://fug.zhongyouzk.top

================================================================================
来源：http://xxc.yongpay.top

[S01] C：Hello World
来源：http://skq.tanke756.top

#include <stdio.h>
来源：http://xuq.ydjk.org.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://akg.9152youxi.cn

[S02] C：变量与格式化输出
来源：http://rqr.hongshengwenyu.top

int a = 10; printf("%d\n", a);
来源：http://jdf.zhaomingkeji.xyz

[S03] C：读入整数
来源：http://eyg.hongshengwenyu.top

int x; scanf("%d", &x);
来源：http://yui.wangdashe.top

[S04] C：字符串复制
来源：http://pfw.redwolf501.top

char dst[32]; strcpy(dst, "hi");
来源：http://auc.yfazqb.com

[S05] C：字符串长度
来源：http://gki.yonumen.top

strlen(s)
来源：http://vkd.xylfe.cn

[S06] C：字符串比较
来源：http://dtd.daxiang520.top

strcmp(a, b) == 0
来源：http://wyi.tianlin.xyz

[S07] C：数组遍历求和
来源：http://eea.bjfxy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xje.zhaomingkeji.xyz

[S08] C：动态内存分配与释放
来源：http://znz.52xcode.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gcg.tian-w.cn

[S09] C：结构体定义与初始化
来源：http://ajj.nanxinkj.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gnq.fzhhl.top

[S10] C：指针与解引用
来源：http://ois.chenzaomai.com

int *p = &a;  *p = 5;
来源：http://ubz.zhiwuduotai.top

[S11] C：逐行读文件
来源：http://zvg.xylfe.cn

FILE *f = fopen("a.txt", "r");
来源：http://auk.fehbvm.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://plw.9152youxi.cn

fclose(f);
来源：http://uwr.zhengqikj.top

[S12] C：写文件
来源：http://xjx.zhongyouzk.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vct.zhongyouzk.top

[S13] C：宏定义
来源：http://wts.ywan-chungtsiang.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://frx.zhoulong.xyz

[S14] C：枚举
来源：http://xlh.bbcook.cn

enum Color { RED, GREEN, BLUE };
来源：http://blh.sufxvd.cn

[S15] C：类型转换
来源：http://njl.yj20258.top

(double) a / b
来源：http://fnr.svipenyu.cn

[S16] C：位操作置位
来源：http://inf.yuanzhike.top

x |= (1 << 3);
来源：http://rxr.yueranfly.top

[S17] C：安全拼接字符串
来源：http://edy.vqdsnc.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vcr.bbcook.cn

[S18] C：命令行参数
来源：http://ljs.zdbjq.cn

int main(int argc, char **argv)
来源：http://fee.shzxlz.cn

[S19] C：快速排序
来源：http://eeq.yj20258.top

qsort(a, n, sizeof(int), cmp);
来源：http://tcd.jiagoushi.top

[S20] C：二分查找
来源：http://vtd.xuanzx.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jzf.yj202588.top

[S21] C：字符类别判断
来源：http://cqs.daxiang520.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xxs.hesvh.cn

[S22] C：字符串转数字
来源：http://tjg.zhongyouzk.top


<!-- 参考信息 -->