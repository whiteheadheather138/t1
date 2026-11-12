代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://bwf.yangfankeji.com

[Q52] 删除指定行
来源：http://jhz.havefunace.top

DELETE FROM users WHERE id = 10;
来源：http://mwf.zhoulong.xyz

[Q53] 按条件删除
来源：http://lvx.shangyingyoupin.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://rzd.hcnkem.com

[Q54] 清空表
来源：http://qsk.ydjk.org.cn

TRUNCATE TABLE logs;
来源：http://bgn.vqdsnc.cn

[Q55] 排名（并列占位）
来源：http://scp.sjlbkw.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://fdg.hnqzz.top

[Q56] 密集排名（并列不占位）
来源：http://knf.bbcook.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://pgn.vqdsnc.cn

[Q57] 行号
来源：http://aql.nanxuanxn.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://inh.meibo888.top

[Q58] 累计求和
来源：http://wzw.jqgufenzy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://cbv.yj20258.top

[Q59] 分组内累计
来源：http://wsh.daxiang520.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://jyt.hesvh.cn

[Q60] 取上一行 / 下一行
来源：http://dum.uphjek.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yua.316326.xyz

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sbm.redwolf501.top

[Q61] 移动平均
来源：http://ujh.zycfv.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://fdh.ydjk.org.cn

[Q62] 分组占比
来源：http://yth.gogol.net.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://gbx.xingfuxueyuan.xyz

[Q63] 开启事务
来源：http://oks.quarkkingdee.top

START TRANSACTION;                -- 或 BEGIN
来源：http://gfi.xingfuxueyuan.xyz

[Q64] 提交事务
来源：http://wdh.snrcjt.cn

COMMIT;
来源：http://ubx.sweek.top

[Q65] 回滚事务
来源：http://zdd.hysaishi.cn

ROLLBACK;
来源：http://xac.nanxuanxn.top

[Q66] 行锁查询
来源：http://ohw.jqgufenzy.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tqu.52xcode.cn

[Q67] 设置隔离级别
来源：http://itk.shuidangran.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kyp.yuxming.cn

[Q68] 保存点
来源：http://chl.sufxvd.cn

SAVEPOINT sp1;
来源：http://ihb.jianghu66.top

ROLLBACK TO sp1;
来源：http://ahe.gaohongyu789.top

[Q69] 查看执行计划
来源：http://txi.yonumen.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nbh.aibaodan.cn

[Q70] 更新统计信息
来源：http://vsw.tarul.cn

ANALYZE TABLE users;
来源：http://cie.smart0.xyz

[Q71] 查看建表语句
来源：http://ppc.gotoacloud.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://kgq.mhx1999.top

[Q72] 查看索引
来源：http://yev.jianghu66.top

SHOW INDEX FROM users;
来源：http://rsf.yj20258.top

[Q73] 查看表状态
来源：http://ppz.yj202588.top

SHOW TABLE STATUS LIKE 'users';
来源：http://qki.wangdashe.top

[Q74] 强制使用索引
来源：http://cax.jiagoushi.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://xcw.yangfankeji.com

[Q75] 日期格式化
来源：http://ptg.snrcjt.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://evm.snrcjt.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ott.guannengcc.top

[Q76] 按天统计
来源：http://mxf.shzxlz.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://upd.xziqi.cn

[Q77] 时间加减
来源：http://mul.jinghuilouyu.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jwx.0kj1m.cn

[Q78] 当前时间
来源：http://euu.yanxiufei.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://scx.hcnkem.com

[Q79] 字符串拼接
来源：http://jlx.jinqigfzy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uit.wangdashe.top

[Q80] 字符串截取
来源：http://xia.xingfuxueyuan.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://svv.hysaishi.cn

[Q81] 字符串替换
来源：http://zbg.shanyushiyangtech.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://axu.cheryme.top

[Q82] 字符长度与字节长度
来源：http://daa.cashguo.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lih.ctjpmb.com

[Q83] 大小写转换
来源：http://pwt.hcnkem.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qeh.ydjk.org.cn

[Q84] 去除首尾空格
来源：http://ich.chenjidiqi.icu

SELECT TRIM(name) FROM users;
来源：http://sow.yj202588.top

[Q85] 数值取整
来源：http://thf.svipenyu.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://rmv.ywan-chungtsiang.top

[Q86] 读取 JSON 字段
来源：http://mye.meibo888.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oza.sxryk.cn

[Q87] JSON 字段做条件
来源：http://glw.gzhubu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://iyp.9152youxi.cn

[Q88] 行转列（条件聚合）
来源：http://zrz.jinqigufen.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://cmq.sufxvd.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://bud.epnwcf.com

[Q89] 判断表是否存在
来源：http://edk.dianchejie.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rtj.gaohongyu789.top

[Q90] 生成序号列
来源：http://bxl.pycfn.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://uij.uphjek.com

================================================================================
来源：http://csq.hesvh.cn

R. Bash 专题
来源：http://xpd.hnqzz.top

================================================================================
来源：http://cny.zdbjq.cn

[R01] shebang 与严格模式
来源：http://viy.fengsongda.top

#!/usr/bin/env bash
来源：http://dji.bbcook.cn

set -euo pipefail
来源：http://mve.xinyue.icu

[R02] 变量赋值与使用
来源：http://ihh.hcnkem.com

name="Tom"; echo "$name"
来源：http://mlt.fehbvm.com

[R03] 只读变量
来源：http://lio.gotoacloud.top

readonly PI=3.14
来源：http://yno.chenlongwang.top

[R04] 位置参数
来源：http://tdi.zhongyouzk.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://otg.pycfn.com

[R05] 参数默认值
来源：http://cfu.zdqjudy.top

name="${1:-default}"
来源：http://fbs.tarul.cn

[R06] 判断命令是否存在
来源：http://ngx.xuanzx.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ebk.fktsv.cn

[R07] if 判断文件
来源：http://wcb.fehbvm.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vyl.yuanzhike.top

[R08] 数值比较
来源：http://aqv.zhengqikj.top

if (( a > b )); then echo "a 更大"; fi
来源：http://uxb.shanyushiyangkeji.top

[R09] 字符串比较
来源：http://apr.fanxiaobao.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://lgg.chenzaomai.com

[R10] 正则匹配
来源：http://zhp.sweek.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://jul.hnqzz.top

[R11] case 多分支
来源：http://rwl.xylfe.cn

case "$1" in
来源：http://jvv.hnxiangtu.top

start) echo "启动" ;;
来源：http://dts.gaohongyu789.top

stop)  echo "停止" ;;
来源：http://wsp.shanyushiyangtech.top

*)     echo "未知命令" ;;
来源：http://bxr.gogol.net.cn

esac
来源：http://kzz.yj202588.top

[R12] for 遍历文件
来源：http://fxa.ivvv.top

for f in *.txt; do echo "$f"; done
来源：http://ofy.zhengqikj.top

[R13] for 计数循环
来源：http://rwp.yj20258888.top

for i in {1..10}; do echo "$i"; done
来源：http://wie.meibo888.top

[R14] C 风格 for
来源：http://bcs.ybcxt.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://tjs.uphjek.com

[R15] while 逐行读文件
来源：http://fuf.hfpthk.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qvt.yfazqb.com

[R16] until 等待条件
来源：http://vug.fktsv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://maq.52xcode.cn

[R17] 数组定义与取值
来源：http://mgd.ehwqpu.com

arr=(a b c); echo "${arr[0]}"
来源：http://ncv.vqdsnc.cn

[R18] 遍历数组
来源：http://wec.yuxming.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ots.andypj.xyz

[R19] 数组长度
来源：http://ovt.yueranfly.top

echo "${#arr[@]}"
来源：http://yyj.cucudq.cn

[R20] 关联数组（字典）
来源：http://pps.yangfankeji.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://uel.hfpthk.cn

[R21] 字符串长度
来源：http://pbt.fktsv.cn

echo "${#s}"
来源：http://yap.xinyue.icu

[R22] 截取子串
来源：http://waq.pengpengdd.cyou

echo "${s:0:5}"
来源：http://njn.kuanghao11.cn

[R23] 字符串替换
来源：http://dyo.yongpay.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://qgb.xylfe.cn

[R24] 大小写转换
来源：http://xbt.gzhubu.top

echo "${s^^}"; echo "${s,,}"
来源：http://sjb.shzxlz.cn

[R25] 去后缀 / 去前缀
来源：http://opb.nanxinkj.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://vtw.gogol.net.cn

[R26] 命令替换
来源：http://lvq.jinyuanbaomall.cn

now=$(date +%F); echo "$now"
来源：http://bwb.shanyushiyangtech.top

[R27] 算术展开
来源：http://bkg.52xcode.cn

echo $((1 + 2 * 3))
来源：http://rre.xziqi.cn

[R28] 浮点运算
来源：http://ejj.sxryk.cn

echo "scale=2; 10/3" | bc
来源：http://klt.yuxming.cn

[R29] 定义函数
来源：http://pog.nanxuanxn.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ucs.zhengqikj.top

[R30] 函数返回状态码
来源：http://rcx.hywenlv.cn

f() { return 0; }; f || echo "失败了"
来源：http://huf.yfazqb.com

[R31] 局部变量
来源：http://mvc.yuanzhike.top

f() { local x=1; echo "$x"; }
来源：http://cic.tanke756.top

[R32] 参数个数校验
来源：http://dic.zhiwuduotai.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xan.gaohongyu789.top

[R33] 捕获错误并提示行号
来源：http://irb.xziqi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mzg.shanyushiyangtech.top

[R34] 退出时清理
来源：http://jnm.wangdashe.top

trap 'rm -f "$tmp"' EXIT
来源：http://inx.quarkkingdee.top

[R35] 后台执行并等待
来源：http://qaw.yanxiufei.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ugj.zhijiandao.cn

[R36] 并发执行多个任务
来源：http://nwy.gogol.net.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xvs.shuidangran.top

[R37] 把输出赋给变量
来源：http://ufg.sysykeji.top

files=$(ls -1)
来源：http://thn.redwolf501.top

[R38] 管道串联
来源：http://lax.shanyushiyangkeji.top

cat a.txt | grep -i error | wc -l
来源：http://pmj.cashguo.top

[R39] 重定向标准输出与错误
来源：http://tzl.redwolf501.top

cmd > out.log 2>&1
来源：http://ukz.shuidangran.top

[R40] 追加写日志
来源：http://jjm.yj20258888.top

echo "log" >> out.log
来源：http://yxh.nanxinkj.top

[R41] 丢弃输出
来源：http://isa.sufxvd.cn

cmd >/dev/null 2>&1
来源：http://iuf.jqgufenzy.top

[R42] 输入重定向
来源：http://hvz.cashguo.top

wc -l < a.txt
来源：http://hjq.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://twk.ehwqpu.com

find . -name "*.log" -type f
来源：http://cud.pengpengdd.cyou

[R44] 按修改时间查找
来源：http://axz.dashuyun.cn

find . -mtime -7 -type f
来源：http://tnw.hysaishi.cn

[R45] 批量删除
来源：http://vre.quarkkingdee.top

find . -name "*.tmp" -delete
来源：http://fec.gaohongyu789.top

[R46] 递归替换文件内容
来源：http://ogc.yueranfly.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tkq.uphjek.com

[R47] sed 单行替换
来源：http://ork.hysaishi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://lyk.nanxinkj.top

[R48] awk 取指定列
来源：http://aky.pycfn.com

awk '{print $1, $3}' a.txt
来源：http://wun.hnxiangtu.top

[R49] awk 带条件
来源：http://lud.jiagoushi.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://xlx.hysaishi.cn

[R50] awk 求和
来源：http://ohq.gogol.net.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zkn.yuxming.cn

[R51] 排序去重取前几
来源：http://muz.hysaishi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xrk.kuanghao11.cn

[R52] 统计行数
来源：http://tdl.xylfe.cn

wc -l a.txt
来源：http://gti.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://inv.jianghu66.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wyr.epnwcf.com

[R54] 比较两个文件
来源：http://zib.pycfn.com

diff a.txt b.txt
来源：http://qyz.ydzc1.top

[R55] 压缩与解压
来源：http://qhn.bbcook.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xwn.tanke756.top

[R56] 远程拷贝
来源：http://vep.jqgfzy.top

scp file user@host:/path/
来源：http://wye.hnxiangtu.top

[R57] 远程执行命令
来源：http://cgk.ybcxt.top

ssh user@host 'uptime'
来源：http://kwe.zhoulong.xyz

[R58] 下载文件
来源：http://usl.fanxiaobao.xyz

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wft.jlsjyb.cn

[R59] 发 POST JSON
来源：http://yfe.jinghuilouyu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hta.shzxlz.cn

[R60] 只看 HTTP 状态码
来源：http://cfx.yfazqb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rco.ydzc1.top

[R61] 磁盘占用
来源：http://ybl.aibaodan.cn

df -h;  du -sh *
来源：http://phh.fehbvm.com

[R62] 找最占空间的文件
来源：http://qyp.havefunace.top

du -ah . | sort -rh | head -10
来源：http://dvy.jlsjyb.cn

[R63] 内存与进程
来源：http://wnm.nanxinkj.top

free -h;  ps aux | grep nginx
来源：http://kdq.smart0.xyz

[R64] 结束进程
来源：http://zaj.kuanghao11.cn

kill -9 $(pgrep -f app.py)
来源：http://xhn.zhijiandao.cn

[R65] 查看端口占用
来源：http://udb.hesvh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fck.meibo888.top

[R66] 定时任务
来源：http://zrh.iojbl.cn

crontab -e;  crontab -l
来源：http://kpe.fehbvm.com

[R67] 生成随机十六进制串
来源：http://qgn.jianghu66.top

openssl rand -hex 16
来源：http://who.kuanghao11.cn

[R68] 计算文件校验值
来源：http://dqo.zhoulong.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://vsp.meibo888.top

[R69] 生成随机密码
来源：http://eel.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://oye.sufxvd.cn

[R70] 时间戳与互转
来源：http://mwf.ydzc1.top

date +%s;  date -d @1700000000
来源：http://sfl.shanyushiyangkeji.top

[R71] 日期格式化
来源：http://gbh.gogol.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xgf.zhiwuduotai.top

[R72] 等待端口就绪
来源：http://tbk.shanyushiyangtech.top

until nc -z localhost 3306; do sleep 1; done
来源：http://geb.ywan-chungtsiang.top

[R73] 分割大日志
来源：http://qjj.jianghu66.top

split -l 1000 big.log part_
来源：http://jhz.sjlbkw.cn

[R74] 批量重命名
来源：http://ifi.aizwys.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xwd.yj20258888.top

[R75] 导出环境变量
来源：http://woq.9152youxi.cn

export PATH="$HOME/bin:$PATH"
来源：http://yya.jinghuilouyu.cn

[R76] 使用临时文件
来源：http://xbx.meibo888.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ujl.hfpthk.cn

[R77] 读取用户输入
来源：http://ueb.hongshengwenyu.top

read -rp "请输入: " ans
来源：http://qkf.haohaochexian.top

[R78] 交互式菜单
来源：http://iku.ivvv.top

select opt in a b c; do echo "$opt"; break; done
来源：http://iqf.fanxiaobao.xyz

[R79] 解析命令行选项
来源：http://try.gotoacloud.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ikf.iojbl.cn

[R80] 查看脚本执行耗时
来源：http://xxu.fengsongda.top

time ./run.sh
来源：http://cah.svipenyu.cn

================================================================================
来源：http://jev.yongpay.top

S. C / C++ 专题
来源：http://scz.gogol.net.cn

================================================================================
来源：http://agy.mhx1999.top

[S01] C：Hello World
来源：http://tys.0kj1m.cn

#include <stdio.h>
来源：http://kwl.jyoumei.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://hwe.shanyushiyangtech.top

[S02] C：变量与格式化输出
来源：http://why.andypj.xyz

int a = 10; printf("%d\n", a);
来源：http://mxw.tanke756.top

[S03] C：读入整数
来源：http://jvx.zycfv.cn

int x; scanf("%d", &x);
来源：http://gwu.hammf.cn

[S04] C：字符串复制
来源：http://adl.jyoumei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hqr.hysaishi.cn

[S05] C：字符串长度
来源：http://vbt.ydjk.org.cn

strlen(s)
来源：http://uzo.jlsjyb.cn

[S06] C：字符串比较
来源：http://xpy.chenzaomai.com

strcmp(a, b) == 0
来源：http://wum.tarul.cn

[S07] C：数组遍历求和
来源：http://nnz.svipenyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://bbd.gotoacloud.top

[S08] C：动态内存分配与释放
来源：http://fiy.uphjek.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rju.quarkkingdee.top

[S09] C：结构体定义与初始化
来源：http://ede.zhongyouzk.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gud.haohaochexian.top

[S10] C：指针与解引用
来源：http://qin.jinghuilouyu.cn

int *p = &a;  *p = 5;
来源：http://bir.haohaochexian.top

[S11] C：逐行读文件
来源：http://tfp.xinyue.icu

FILE *f = fopen("a.txt", "r");
来源：http://qyg.jqgufenzy.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://wbp.nanxuanxn.top

fclose(f);
来源：http://ysz.0kj1m.cn

[S12] C：写文件
来源：http://les.shanyushiyangkeji.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sma.uphjek.com

[S13] C：宏定义
来源：http://kay.hesvh.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bep.sufxvd.cn

[S14] C：枚举
来源：http://yrs.birdmap.top

enum Color { RED, GREEN, BLUE };
来源：http://foh.ctjpmb.com

[S15] C：类型转换
来源：http://hkg.jinqigfzy.top

(double) a / b
来源：http://jhn.fengsongda.top

[S16] C：位操作置位
来源：http://xwt.aibaodan.cn

x |= (1 << 3);
来源：http://wgc.pengpengdd.cyou

[S17] C：安全拼接字符串
来源：http://yba.smart0.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://csz.yvedp.cn

[S18] C：命令行参数
来源：http://lrl.iojbl.cn

int main(int argc, char **argv)
来源：http://ejv.gaohongyu789.top

[S19] C：快速排序
来源：http://ade.bbcook.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ycp.guowangkeji.top

[S20] C：二分查找
来源：http://gyz.hywenlv.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gjr.mhx1999.top

[S21] C：字符类别判断
来源：http://quy.tarul.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://frq.quarkkingdee.top

[S22] C：字符串转数字
来源：http://ocm.zhongyouzk.top


<!-- 参考信息 -->