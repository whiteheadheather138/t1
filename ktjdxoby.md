代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://obv.shuidangran.top

[Q52] 删除指定行
来源：http://yvn.ivvv.top

DELETE FROM users WHERE id = 10;
来源：http://jfc.daxiang520.top

[Q53] 按条件删除
来源：http://kna.tanke756.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gby.zhaomingkeji.xyz

[Q54] 清空表
来源：http://yvt.sxryk.cn

TRUNCATE TABLE logs;
来源：http://qzc.daria6918.cn

[Q55] 排名（并列占位）
来源：http://amz.ywan-chungtsiang.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://jym.gogol.net.cn

[Q56] 密集排名（并列不占位）
来源：http://taq.fktsv.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://eyx.fzhhl.top

[Q57] 行号
来源：http://yqs.cqqwz.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://lcj.mhx1999.top

[Q58] 累计求和
来源：http://oho.xziqi.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ozf.pengpengdd.cyou

[Q59] 分组内累计
来源：http://wvn.fktsv.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pyg.sjlbkw.cn

[Q60] 取上一行 / 下一行
来源：http://rzl.nanxuanxn.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://kqz.uphjek.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wdp.zhixingplan.top

[Q61] 移动平均
来源：http://puq.jinqigufen.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://cyr.shzxlz.cn

[Q62] 分组占比
来源：http://bhk.shanyushiyangtech.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ccu.yj20258.top

[Q63] 开启事务
来源：http://afe.yonumen.top

START TRANSACTION;                -- 或 BEGIN
来源：http://pld.andypj.xyz

[Q64] 提交事务
来源：http://eup.dianchejie.cn

COMMIT;
来源：http://gmv.xylfe.cn

[Q65] 回滚事务
来源：http://luh.jinqigufen.top

ROLLBACK;
来源：http://jen.tianlin.xyz

[Q66] 行锁查询
来源：http://mtg.0kj1m.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://rlg.jinyuanbaomall.cn

[Q67] 设置隔离级别
来源：http://wrq.birdmap.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://yyl.bjfxy.top

[Q68] 保存点
来源：http://aeo.jiagoushi.top

SAVEPOINT sp1;
来源：http://lrp.gaohongyu789.top

ROLLBACK TO sp1;
来源：http://fic.ivvv.top

[Q69] 查看执行计划
来源：http://saf.yj202588.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://nxn.yj202588.top

[Q70] 更新统计信息
来源：http://zqp.cheryme.top

ANALYZE TABLE users;
来源：http://acx.zhoulong.xyz

[Q71] 查看建表语句
来源：http://xug.hesvh.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://zbu.meibo888.top

[Q72] 查看索引
来源：http://tte.hnxiangtu.top

SHOW INDEX FROM users;
来源：http://jtj.redwolf501.top

[Q73] 查看表状态
来源：http://ypg.yj202588.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ayh.ywan-chungtsiang.top

[Q74] 强制使用索引
来源：http://oko.9152youxi.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://gvc.hysaishi.cn

[Q75] 日期格式化
来源：http://ovf.zhoulong.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yyv.shzxlz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://fwd.shzxlz.cn

[Q76] 按天统计
来源：http://lnq.yuanzhike.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://emh.fengsongda.top

[Q77] 时间加减
来源：http://eww.hammf.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://zbe.ctjpmb.com

[Q78] 当前时间
来源：http://wlv.yj20258888.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://qvg.yvedp.cn

[Q79] 字符串拼接
来源：http://cvn.svipenyu.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uxh.ehwqpu.com

[Q80] 字符串截取
来源：http://vxq.aibaodan.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ssj.fktsv.cn

[Q81] 字符串替换
来源：http://ssd.ppjwa.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://csw.hesvh.cn

[Q82] 字符长度与字节长度
来源：http://oiq.tianlin.xyz

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rij.c1oappe.top

[Q83] 大小写转换
来源：http://zlj.epnwcf.com

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sew.hammf.cn

[Q84] 去除首尾空格
来源：http://fbk.bbcook.cn

SELECT TRIM(name) FROM users;
来源：http://bhr.nanxuanxn.top

[Q85] 数值取整
来源：http://fhw.xylfe.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://xbk.nwbrower.top

[Q86] 读取 JSON 字段
来源：http://zun.xuanzx.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://vxg.hywenlv.cn

[Q87] JSON 字段做条件
来源：http://omq.zhixingplan.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://csu.hfpthk.cn

[Q88] 行转列（条件聚合）
来源：http://utp.xziqi.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://dmi.pengpengdd.cyou

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://qor.tarul.cn

[Q89] 判断表是否存在
来源：http://oxp.ywan-chungtsiang.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://jfj.zdqjudy.top

[Q90] 生成序号列
来源：http://jjr.chenlongwang.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jex.xingfuxueyuan.xyz

================================================================================
来源：http://vjl.xziqi.cn

R. Bash 专题
来源：http://oxz.gotoacloud.top

================================================================================
来源：http://nae.xylfe.cn

[R01] shebang 与严格模式
来源：http://qix.pycfn.com

#!/usr/bin/env bash
来源：http://ujx.daria6918.cn

set -euo pipefail
来源：http://xms.xuanzx.com

[R02] 变量赋值与使用
来源：http://wzb.gzhubu.top

name="Tom"; echo "$name"
来源：http://vsm.zhijiandao.cn

[R03] 只读变量
来源：http://eup.daxiang520.top

readonly PI=3.14
来源：http://uke.jlsjyb.cn

[R04] 位置参数
来源：http://wdz.cucudq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qys.hesvh.cn

[R05] 参数默认值
来源：http://awo.andypj.xyz

name="${1:-default}"
来源：http://rqf.ybcxt.top

[R06] 判断命令是否存在
来源：http://irz.ybcxt.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://jay.andypj.xyz

[R07] if 判断文件
来源：http://ddk.guowangkeji.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://rdl.jqgfzy.top

[R08] 数值比较
来源：http://pzj.xziqi.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xkv.sufxvd.cn

[R09] 字符串比较
来源：http://yak.c1oappe.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jti.hcnkem.com

[R10] 正则匹配
来源：http://owy.meibo888.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://grr.sxryk.cn

[R11] case 多分支
来源：http://vie.gogol.net.cn

case "$1" in
来源：http://rxk.ppjwa.cn

start) echo "启动" ;;
来源：http://bbt.hesvh.cn

stop)  echo "停止" ;;
来源：http://tkz.cqqwz.cn

*)     echo "未知命令" ;;
来源：http://zge.mhx1999.top

esac
来源：http://tqf.sjlbkw.cn

[R12] for 遍历文件
来源：http://qcz.jinyuanbaomall.cn

for f in *.txt; do echo "$f"; done
来源：http://oiq.kuanghao11.cn

[R13] for 计数循环
来源：http://shl.aibaodan.cn

for i in {1..10}; do echo "$i"; done
来源：http://uoz.hcnkem.com

[R14] C 风格 for
来源：http://lqa.hcnkem.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jfn.cdnleiting.top

[R15] while 逐行读文件
来源：http://heq.chenjidiqi.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ccy.jinghuilouyu.cn

[R16] until 等待条件
来源：http://nkr.jlsjyb.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qtr.xziqi.cn

[R17] 数组定义与取值
来源：http://ayw.fktsv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://zyk.epnwcf.com

[R18] 遍历数组
来源：http://spy.shangyingyoupin.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://tim.hesvh.cn

[R19] 数组长度
来源：http://mwq.shanyushiyangtech.top

echo "${#arr[@]}"
来源：http://ogx.meibo888.top

[R20] 关联数组（字典）
来源：http://mii.yvedp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://rmi.gzhubu.top

[R21] 字符串长度
来源：http://vjy.yj20258888.top

echo "${#s}"
来源：http://iqc.cdnleiting.top

[R22] 截取子串
来源：http://ukz.ybcxt.top

echo "${s:0:5}"
来源：http://pen.xuetiantiany.cn

[R23] 字符串替换
来源：http://fhm.zhengqikj.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gmr.sysykeji.top

[R24] 大小写转换
来源：http://cek.yongpay.top

echo "${s^^}"; echo "${s,,}"
来源：http://mup.chenjidiqi.icu

[R25] 去后缀 / 去前缀
来源：http://nut.shanyushiyangtech.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://wcj.hfpthk.cn

[R26] 命令替换
来源：http://sko.jqgfzy.top

now=$(date +%F); echo "$now"
来源：http://cgw.daria6918.cn

[R27] 算术展开
来源：http://hrn.yonumen.top

echo $((1 + 2 * 3))
来源：http://uku.zycfv.cn

[R28] 浮点运算
来源：http://tia.zhiwuduotai.top

echo "scale=2; 10/3" | bc
来源：http://prt.pengpengdd.cyou

[R29] 定义函数
来源：http://isr.wangdashe.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://frz.yfazqb.com

[R30] 函数返回状态码
来源：http://nuj.jianghu66.top

f() { return 0; }; f || echo "失败了"
来源：http://eca.snrcjt.cn

[R31] 局部变量
来源：http://iub.jqgfzy.top

f() { local x=1; echo "$x"; }
来源：http://yix.hywenlv.cn

[R32] 参数个数校验
来源：http://syu.hammf.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://gtz.yfazqb.com

[R33] 捕获错误并提示行号
来源：http://mdl.gaohongyu789.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qkm.52xcode.cn

[R34] 退出时清理
来源：http://kbf.yj202588.top

trap 'rm -f "$tmp"' EXIT
来源：http://wuz.zhixingplan.top

[R35] 后台执行并等待
来源：http://mcn.quarkkingdee.top

sleep 5 & pid=$!; wait "$pid"
来源：http://gvi.tanke756.top

[R36] 并发执行多个任务
来源：http://jbw.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mhp.jqgufenzy.top

[R37] 把输出赋给变量
来源：http://drj.zhijiandao.cn

files=$(ls -1)
来源：http://jlv.yj20258888.top

[R38] 管道串联
来源：http://eyr.cqqwz.cn

cat a.txt | grep -i error | wc -l
来源：http://xnv.hysaishi.cn

[R39] 重定向标准输出与错误
来源：http://tpy.xuetiantiany.cn

cmd > out.log 2>&1
来源：http://oni.ywan-chungtsiang.top

[R40] 追加写日志
来源：http://tbm.zhongyouzk.top

echo "log" >> out.log
来源：http://qfo.tian-w.cn

[R41] 丢弃输出
来源：http://mnu.ctjpmb.com

cmd >/dev/null 2>&1
来源：http://vxb.cheryme.top

[R42] 输入重定向
来源：http://dpm.daxiang520.top

wc -l < a.txt
来源：http://fgm.nwbrower.top

[R43] 按名字查找文件
来源：http://yjn.guannengcc.top

find . -name "*.log" -type f
来源：http://npk.svipenyu.cn

[R44] 按修改时间查找
来源：http://txh.nwbrower.top

find . -mtime -7 -type f
来源：http://rvg.xuetiantiany.cn

[R45] 批量删除
来源：http://mir.epnwcf.com

find . -name "*.tmp" -delete
来源：http://ggj.shuidangran.top

[R46] 递归替换文件内容
来源：http://wou.zhaomingkeji.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://kzn.vqdsnc.cn

[R47] sed 单行替换
来源：http://shv.yj20258888.top

sed -i 's/foo/bar/g' a.txt
来源：http://iwi.zhijiandao.cn

[R48] awk 取指定列
来源：http://gsd.tian-w.cn

awk '{print $1, $3}' a.txt
来源：http://hyc.jlsjyb.cn

[R49] awk 带条件
来源：http://pvr.yvedp.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://nlv.ybcxt.top

[R50] awk 求和
来源：http://mwu.hnqzz.top

awk '{s += $2} END {print s}' a.txt
来源：http://zgv.tanke756.top

[R51] 排序去重取前几
来源：http://zoj.ydzc1.top

sort a.txt | uniq -c | sort -rn | head
来源：http://imt.zhiwuduotai.top

[R52] 统计行数
来源：http://gwz.yanxiufei.cn

wc -l a.txt
来源：http://pce.zhongyouzk.top

[R53] 查看文件头与实时尾
来源：http://egl.fengsongda.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://scc.jinqigfzy.top

[R54] 比较两个文件
来源：http://zhk.tarul.cn

diff a.txt b.txt
来源：http://qby.zhaomingkeji.xyz

[R55] 压缩与解压
来源：http://gsz.smart0.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hgm.cucudq.cn

[R56] 远程拷贝
来源：http://yjt.jiagoushi.top

scp file user@host:/path/
来源：http://tfo.cashguo.top

[R57] 远程执行命令
来源：http://ekm.sufxvd.cn

ssh user@host 'uptime'
来源：http://bzf.kuanghao11.cn

[R58] 下载文件
来源：http://ddj.birdmap.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wfm.haohaochexian.top

[R59] 发 POST JSON
来源：http://gra.mhx1999.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ibx.jiagoushi.top

[R60] 只看 HTTP 状态码
来源：http://nxj.zhiwuduotai.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mwt.aizwys.cn

[R61] 磁盘占用
来源：http://tpn.zhongyouzk.top

df -h;  du -sh *
来源：http://eik.epnwcf.com

[R62] 找最占空间的文件
来源：http://nsw.yfazqb.com

du -ah . | sort -rh | head -10
来源：http://nhc.hnxiangtu.top

[R63] 内存与进程
来源：http://txb.daxiang520.top

free -h;  ps aux | grep nginx
来源：http://jog.gogol.net.cn

[R64] 结束进程
来源：http://zxq.zhengqikj.top

kill -9 $(pgrep -f app.py)
来源：http://bjl.cheryme.top

[R65] 查看端口占用
来源：http://avb.jlsjyb.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xgl.ybcxt.top

[R66] 定时任务
来源：http://tnq.fzhhl.top

crontab -e;  crontab -l
来源：http://zvi.shanyushiyangtech.top

[R67] 生成随机十六进制串
来源：http://pwn.jyoumei.cn

openssl rand -hex 16
来源：http://pbz.cashguo.top

[R68] 计算文件校验值
来源：http://yoz.yvedp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sbz.zdbjq.cn

[R69] 生成随机密码
来源：http://fhu.jlsjyb.cn

head -c 16 /dev/urandom | base64
来源：http://vdw.hongshengwenyu.top

[R70] 时间戳与互转
来源：http://qkf.jinyuanbaomall.cn

date +%s;  date -d @1700000000
来源：http://djh.wangshuangyany.cn

[R71] 日期格式化
来源：http://fkc.chenzaomai.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://zrs.sjlbkw.cn

[R72] 等待端口就绪
来源：http://tnk.yonumen.top

until nc -z localhost 3306; do sleep 1; done
来源：http://tmq.tarul.cn

[R73] 分割大日志
来源：http://ufr.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://ggv.xziqi.cn

[R74] 批量重命名
来源：http://bmb.daria6918.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cal.gogol.net.cn

[R75] 导出环境变量
来源：http://evo.gogol.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://sii.zdqjudy.top

[R76] 使用临时文件
来源：http://xyy.chenlongwang.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lyg.hnxiangtu.top

[R77] 读取用户输入
来源：http://xxu.yangfankeji.com

read -rp "请输入: " ans
来源：http://bzi.sxryk.cn

[R78] 交互式菜单
来源：http://snt.hywenlv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tnt.nanxinkj.top

[R79] 解析命令行选项
来源：http://hhj.yongpay.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eyf.hesvh.cn

[R80] 查看脚本执行耗时
来源：http://til.tarul.cn

time ./run.sh
来源：http://ydb.tian-w.cn

================================================================================
来源：http://eyp.jqgufenzy.top

S. C / C++ 专题
来源：http://ctf.hongshengwenyu.top

================================================================================
来源：http://hjt.zhoulong.xyz

[S01] C：Hello World
来源：http://oxe.nanxinkj.top

#include <stdio.h>
来源：http://qod.yueranfly.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://oro.9152youxi.cn

[S02] C：变量与格式化输出
来源：http://kov.yongpay.top

int a = 10; printf("%d\n", a);
来源：http://mxi.mhx1999.top

[S03] C：读入整数
来源：http://kil.iojbl.cn

int x; scanf("%d", &x);
来源：http://trm.wangshuangyany.cn

[S04] C：字符串复制
来源：http://mml.wangdashe.top

char dst[32]; strcpy(dst, "hi");
来源：http://cym.sufxvd.cn

[S05] C：字符串长度
来源：http://fcg.hfpthk.cn

strlen(s)
来源：http://fsj.bbcook.cn

[S06] C：字符串比较
来源：http://zng.feifeiyinyue.top

strcmp(a, b) == 0
来源：http://yad.nanxinkj.top

[S07] C：数组遍历求和
来源：http://cls.jinghuilouyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kix.andypj.xyz

[S08] C：动态内存分配与释放
来源：http://zer.epnwcf.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://cuk.ydjk.org.cn

[S09] C：结构体定义与初始化
来源：http://gqk.hongshengwenyu.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://azo.haohaochexian.top

[S10] C：指针与解引用
来源：http://ghn.fengsongda.top

int *p = &a;  *p = 5;
来源：http://qpt.tarul.cn

[S11] C：逐行读文件
来源：http://hqo.ppjwa.cn

FILE *f = fopen("a.txt", "r");
来源：http://mfv.cheryme.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://tqs.cqqwz.cn

fclose(f);
来源：http://hfo.nwbrower.top

[S12] C：写文件
来源：http://cah.ctjpmb.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://coo.nanxuanxn.top

[S13] C：宏定义
来源：http://aod.zhaomingkeji.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zzv.yuxming.cn

[S14] C：枚举
来源：http://ort.kuanghao11.cn

enum Color { RED, GREEN, BLUE };
来源：http://oip.nwbrower.top

[S15] C：类型转换
来源：http://luz.birdmap.top

(double) a / b
来源：http://ztb.hywenlv.cn

[S16] C：位操作置位
来源：http://inw.tian-w.cn

x |= (1 << 3);
来源：http://bvp.dashuyun.cn

[S17] C：安全拼接字符串
来源：http://aqn.epnwcf.com

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qus.ehwqpu.com

[S18] C：命令行参数
来源：http://lrp.epnwcf.com

int main(int argc, char **argv)
来源：http://sjy.vehdjk.com

[S19] C：快速排序
来源：http://awi.316326.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://uji.xingfuxueyuan.xyz

[S20] C：二分查找
来源：http://vei.zhixingplan.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wji.xziqi.cn

[S21] C：字符类别判断
来源：http://izc.tian-w.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sbm.haohaochexian.top

[S22] C：字符串转数字
来源：http://swb.yueranfly.top


<!-- 参考信息 -->