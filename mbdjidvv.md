代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://jsp.meibo888.top

[Q54] 清空表
来源：http://ofx.zhixingplan.top

TRUNCATE TABLE logs;
来源：http://psp.fzhhl.top

[Q55] 排名（并列占位）
来源：http://grm.jinqigfzy.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://edr.yonumen.top

[Q56] 密集排名（并列不占位）
来源：http://lrb.ydzc1.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wpo.52xcode.cn

[Q57] 行号
来源：http://bvw.aibaodan.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://its.ydjk.org.cn

[Q58] 累计求和
来源：http://baz.ctjpmb.com

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://acv.jqgfzy.top

[Q59] 分组内累计
来源：http://xjs.bbcook.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://prk.yongpay.top

[Q60] 取上一行 / 下一行
来源：http://pei.birdmap.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://tpv.iojbl.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://lhi.fehbvm.com

[Q61] 移动平均
来源：http://fte.gaohongyu789.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://uju.sufxvd.cn

[Q62] 分组占比
来源：http://cro.xylfe.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://icn.zhijiandao.cn

[Q63] 开启事务
来源：http://hzg.yueranfly.top

START TRANSACTION;                -- 或 BEGIN
来源：http://fvz.zycfv.cn

[Q64] 提交事务
来源：http://dqc.haohaochexian.top

COMMIT;
来源：http://kep.guowangkeji.top

[Q65] 回滚事务
来源：http://pfm.pengpengdd.cyou

ROLLBACK;
来源：http://ein.daria6918.cn

[Q66] 行锁查询
来源：http://soh.vehdjk.com

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://lid.jqgufenzy.top

[Q67] 设置隔离级别
来源：http://ggb.ydjk.org.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://njs.zdqjudy.top

[Q68] 保存点
来源：http://sfj.cheryme.top

SAVEPOINT sp1;
来源：http://vuz.nanxinkj.top

ROLLBACK TO sp1;
来源：http://hxz.jinqigfzy.top

[Q69] 查看执行计划
来源：http://lec.jqgfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zrg.pengpengdd.cyou

[Q70] 更新统计信息
来源：http://hnf.jiagoushi.top

ANALYZE TABLE users;
来源：http://lcf.hnqzz.top

[Q71] 查看建表语句
来源：http://pag.uphjek.com

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qrj.bbcook.cn

[Q72] 查看索引
来源：http://qfj.wangshuangyany.cn

SHOW INDEX FROM users;
来源：http://upq.feifeiyinyue.top

[Q73] 查看表状态
来源：http://lrd.cdnleiting.top

SHOW TABLE STATUS LIKE 'users';
来源：http://drt.hywenlv.cn

[Q74] 强制使用索引
来源：http://kyy.dianchejie.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://yyv.wangdashe.top

[Q75] 日期格式化
来源：http://nqu.fktsv.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://quq.yj20258888.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://xbv.xziqi.cn

[Q76] 按天统计
来源：http://kvz.yuanzhike.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vpt.shangyingyoupin.top

[Q77] 时间加减
来源：http://bvy.daria6918.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nqd.daxiang520.top

[Q78] 当前时间
来源：http://wun.tian-w.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ccs.316326.xyz

[Q79] 字符串拼接
来源：http://mjf.shanyushiyangkeji.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gtu.jqgfzy.top

[Q80] 字符串截取
来源：http://drn.zhengqikj.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://kyf.sweek.top

[Q81] 字符串替换
来源：http://ryr.nanxuanxn.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rnj.meibo888.top

[Q82] 字符长度与字节长度
来源：http://cos.fzhhl.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kyn.ppjwa.cn

[Q83] 大小写转换
来源：http://yra.jinqigfzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://pds.havefunace.top

[Q84] 去除首尾空格
来源：http://vvo.yj20258888.top

SELECT TRIM(name) FROM users;
来源：http://xhd.sweek.top

[Q85] 数值取整
来源：http://sws.pycfn.com

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zpr.zhoulong.xyz

[Q86] 读取 JSON 字段
来源：http://won.yanxiufei.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dqq.meibo888.top

[Q87] JSON 字段做条件
来源：http://ihx.dashuyun.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://qex.yj202588.top

[Q88] 行转列（条件聚合）
来源：http://qjd.jinqigfzy.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ndp.wangdashe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hjm.fanxiaobao.xyz

[Q89] 判断表是否存在
来源：http://goj.andypj.xyz

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://zxg.daxiang520.top

[Q90] 生成序号列
来源：http://mum.tianlin.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://oob.yanxiufei.cn

================================================================================
来源：http://dei.gzhubu.top

R. Bash 专题
来源：http://syi.sysykeji.top

================================================================================
来源：http://tjy.yonumen.top

[R01] shebang 与严格模式
来源：http://nnj.feifeiyinyue.top

#!/usr/bin/env bash
来源：http://gok.havefunace.top

set -euo pipefail
来源：http://hph.xuetiantiany.cn

[R02] 变量赋值与使用
来源：http://btm.ctjpmb.com

name="Tom"; echo "$name"
来源：http://wqe.cheryme.top

[R03] 只读变量
来源：http://qgq.hesvh.cn

readonly PI=3.14
来源：http://zxd.316326.xyz

[R04] 位置参数
来源：http://oyd.sjlbkw.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://jng.jinghuilouyu.cn

[R05] 参数默认值
来源：http://jja.chenjidiqi.icu

name="${1:-default}"
来源：http://phs.jqgufenzy.top

[R06] 判断命令是否存在
来源：http://eau.birdmap.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rag.9152youxi.cn

[R07] if 判断文件
来源：http://sqa.kuanghao11.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://cxz.tian-w.cn

[R08] 数值比较
来源：http://oki.jlsjyb.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xwl.jlsjyb.cn

[R09] 字符串比较
来源：http://jyw.kuanghao11.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zgo.epnwcf.com

[R10] 正则匹配
来源：http://pho.zhoulong.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://cmv.hesvh.cn

[R11] case 多分支
来源：http://jpg.shzxlz.cn

case "$1" in
来源：http://vkd.nanxinkj.top

start) echo "启动" ;;
来源：http://fiz.shzxlz.cn

stop)  echo "停止" ;;
来源：http://nid.birdmap.top

*)     echo "未知命令" ;;
来源：http://sgk.316326.xyz

esac
来源：http://api.yvedp.cn

[R12] for 遍历文件
来源：http://npn.daxiang520.top

for f in *.txt; do echo "$f"; done
来源：http://nhm.dianchejie.cn

[R13] for 计数循环
来源：http://yme.iojbl.cn

for i in {1..10}; do echo "$i"; done
来源：http://frk.ivvv.top

[R14] C 风格 for
来源：http://agp.ctjpmb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qzq.cdnleiting.top

[R15] while 逐行读文件
来源：http://nyc.fanxiaobao.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ebo.ydjk.org.cn

[R16] until 等待条件
来源：http://jgc.zycfv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hef.fzhhl.top

[R17] 数组定义与取值
来源：http://nfn.wangdashe.top

arr=(a b c); echo "${arr[0]}"
来源：http://esi.tian-w.cn

[R18] 遍历数组
来源：http://cju.zhijiandao.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zyo.kuanghao11.cn

[R19] 数组长度
来源：http://glk.xuetiantiany.cn

echo "${#arr[@]}"
来源：http://asq.ywan-chungtsiang.top

[R20] 关联数组（字典）
来源：http://sfs.yvedp.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bhp.svipenyu.cn

[R21] 字符串长度
来源：http://iog.jyoumei.cn

echo "${#s}"
来源：http://dhb.gzhubu.top

[R22] 截取子串
来源：http://dau.cheryme.top

echo "${s:0:5}"
来源：http://egv.cheryme.top

[R23] 字符串替换
来源：http://lue.snrcjt.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://aog.chenlongwang.top

[R24] 大小写转换
来源：http://ocn.ppjwa.cn

echo "${s^^}"; echo "${s,,}"
来源：http://asr.aizwys.cn

[R25] 去后缀 / 去前缀
来源：http://vcr.fanxiaobao.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://gzv.aibaodan.cn

[R26] 命令替换
来源：http://khd.tian-w.cn

now=$(date +%F); echo "$now"
来源：http://led.pengpengdd.cyou

[R27] 算术展开
来源：http://mzg.sweek.top

echo $((1 + 2 * 3))
来源：http://vwv.tanke756.top

[R28] 浮点运算
来源：http://uvg.yongpay.top

echo "scale=2; 10/3" | bc
来源：http://tls.hcnkem.com

[R29] 定义函数
来源：http://tok.tian-w.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gjw.zhongyouzk.top

[R30] 函数返回状态码
来源：http://swp.hnxiangtu.top

f() { return 0; }; f || echo "失败了"
来源：http://cgp.jyoumei.cn

[R31] 局部变量
来源：http://erb.aibaodan.cn

f() { local x=1; echo "$x"; }
来源：http://cuj.uphjek.com

[R32] 参数个数校验
来源：http://kmu.zhaomingkeji.xyz

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://zdw.ydjk.org.cn

[R33] 捕获错误并提示行号
来源：http://rfp.shuidangran.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://eoy.vehdjk.com

[R34] 退出时清理
来源：http://jnc.cheryme.top

trap 'rm -f "$tmp"' EXIT
来源：http://yaf.cqqwz.cn

[R35] 后台执行并等待
来源：http://tgm.cheryme.top

sleep 5 & pid=$!; wait "$pid"
来源：http://deu.feifeiyinyue.top

[R36] 并发执行多个任务
来源：http://gaz.tanke756.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://arn.dashuyun.cn

[R37] 把输出赋给变量
来源：http://nlt.hywenlv.cn

files=$(ls -1)
来源：http://xjl.yanxiufei.cn

[R38] 管道串联
来源：http://cyb.xylfe.cn

cat a.txt | grep -i error | wc -l
来源：http://wlu.fehbvm.com

[R39] 重定向标准输出与错误
来源：http://qkx.fktsv.cn

cmd > out.log 2>&1
来源：http://aml.hfpthk.cn

[R40] 追加写日志
来源：http://bir.jyoumei.cn

echo "log" >> out.log
来源：http://rrb.havefunace.top

[R41] 丢弃输出
来源：http://hfd.fzhhl.top

cmd >/dev/null 2>&1
来源：http://bol.xziqi.cn

[R42] 输入重定向
来源：http://mhi.tarul.cn

wc -l < a.txt
来源：http://qrg.zhaomingkeji.xyz

[R43] 按名字查找文件
来源：http://mjw.quarkkingdee.top

find . -name "*.log" -type f
来源：http://jpp.ehwqpu.com

[R44] 按修改时间查找
来源：http://dyj.yangfankeji.com

find . -mtime -7 -type f
来源：http://cef.jinyuanbaomall.cn

[R45] 批量删除
来源：http://apc.sufxvd.cn

find . -name "*.tmp" -delete
来源：http://qby.shanyushiyangkeji.top

[R46] 递归替换文件内容
来源：http://ewu.daria6918.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://uui.jinqigfzy.top

[R47] sed 单行替换
来源：http://utr.zhoulong.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://hmx.ppjwa.cn

[R48] awk 取指定列
来源：http://uli.zhoulong.xyz

awk '{print $1, $3}' a.txt
来源：http://usx.jinqigufen.top

[R49] awk 带条件
来源：http://nlo.aibaodan.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fua.cucudq.cn

[R50] awk 求和
来源：http://pfp.daxiang520.top

awk '{s += $2} END {print s}' a.txt
来源：http://fgu.gotoacloud.top

[R51] 排序去重取前几
来源：http://vvm.shzxlz.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rfb.yueranfly.top

[R52] 统计行数
来源：http://mlx.hysaishi.cn

wc -l a.txt
来源：http://dqy.hywenlv.cn

[R53] 查看文件头与实时尾
来源：http://iux.yuxming.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iyt.yj20258.top

[R54] 比较两个文件
来源：http://hzg.zdqjudy.top

diff a.txt b.txt
来源：http://lki.tarul.cn

[R55] 压缩与解压
来源：http://obz.gaohongyu789.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://owk.ehwqpu.com

[R56] 远程拷贝
来源：http://gef.nanxuanxn.top

scp file user@host:/path/
来源：http://uxd.andypj.xyz

[R57] 远程执行命令
来源：http://jsc.yvedp.cn

ssh user@host 'uptime'
来源：http://rqi.jlsjyb.cn

[R58] 下载文件
来源：http://alm.zhengqikj.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lth.havefunace.top

[R59] 发 POST JSON
来源：http://pit.gaohongyu789.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://anf.shanyushiyangkeji.top

[R60] 只看 HTTP 状态码
来源：http://axz.zycfv.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oma.feifeiyinyue.top

[R61] 磁盘占用
来源：http://idg.gaohongyu789.top

df -h;  du -sh *
来源：http://mkp.gotoacloud.top

[R62] 找最占空间的文件
来源：http://wdz.ydjk.org.cn

du -ah . | sort -rh | head -10
来源：http://ole.chenjidiqi.icu

[R63] 内存与进程
来源：http://rxy.iojbl.cn

free -h;  ps aux | grep nginx
来源：http://ang.pycfn.com

[R64] 结束进程
来源：http://krh.nanxuanxn.top

kill -9 $(pgrep -f app.py)
来源：http://drp.jinqigufen.top

[R65] 查看端口占用
来源：http://jdx.aizwys.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pok.yuanzhike.top

[R66] 定时任务
来源：http://oyk.daria6918.cn

crontab -e;  crontab -l
来源：http://qlm.nanxuanxn.top

[R67] 生成随机十六进制串
来源：http://crz.jinqigfzy.top

openssl rand -hex 16
来源：http://hrc.birdmap.top

[R68] 计算文件校验值
来源：http://wst.yongpay.top

sha256sum a.txt;  md5sum a.txt
来源：http://acz.fzhhl.top

[R69] 生成随机密码
来源：http://cdq.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://uhm.fzhhl.top

[R70] 时间戳与互转
来源：http://iww.guowangkeji.top

date +%s;  date -d @1700000000
来源：http://grc.ywan-chungtsiang.top

[R71] 日期格式化
来源：http://zqk.cucudq.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fmu.andypj.xyz

[R72] 等待端口就绪
来源：http://reo.guannengcc.top

until nc -z localhost 3306; do sleep 1; done
来源：http://khp.yongpay.top

[R73] 分割大日志
来源：http://pjh.guowangkeji.top

split -l 1000 big.log part_
来源：http://oii.xziqi.cn

[R74] 批量重命名
来源：http://veu.9152youxi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://soh.vehdjk.com

[R75] 导出环境变量
来源：http://udy.haohaochexian.top

export PATH="$HOME/bin:$PATH"
来源：http://lvq.snrcjt.cn

[R76] 使用临时文件
来源：http://bjw.hammf.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bvq.jyoumei.cn

[R77] 读取用户输入
来源：http://opw.zhijiandao.cn

read -rp "请输入: " ans
来源：http://pvs.yanxiufei.cn

[R78] 交互式菜单
来源：http://xtj.xinyue.icu

select opt in a b c; do echo "$opt"; break; done
来源：http://ncu.zhixingplan.top

[R79] 解析命令行选项
来源：http://sht.52xcode.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fdo.zhijiandao.cn

[R80] 查看脚本执行耗时
来源：http://ypk.hammf.cn

time ./run.sh
来源：http://ifa.nanxinkj.top

================================================================================
来源：http://chy.vehdjk.com

S. C / C++ 专题
来源：http://lig.sweek.top

================================================================================
来源：http://xga.yueranfly.top

[S01] C：Hello World
来源：http://avq.jlsjyb.cn

#include <stdio.h>
来源：http://ubw.jqgfzy.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://lex.yuxming.cn

[S02] C：变量与格式化输出
来源：http://xrv.hywenlv.cn

int a = 10; printf("%d\n", a);
来源：http://brq.fengsongda.top

[S03] C：读入整数
来源：http://cqz.tianlin.xyz

int x; scanf("%d", &x);
来源：http://kzy.sjlbkw.cn

[S04] C：字符串复制
来源：http://rgs.jinyuanbaomall.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uwr.yj20258.top

[S05] C：字符串长度
来源：http://wro.jiagoushi.top

strlen(s)
来源：http://lvr.chenjidiqi.icu

[S06] C：字符串比较
来源：http://qcu.ywan-chungtsiang.top

strcmp(a, b) == 0
来源：http://mhc.cqqwz.cn

[S07] C：数组遍历求和
来源：http://int.yongpay.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lpo.jinqigufen.top

[S08] C：动态内存分配与释放
来源：http://wzw.sweek.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dpr.yongpay.top

[S09] C：结构体定义与初始化
来源：http://fnt.pengpengdd.cyou

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jie.guowangkeji.top

[S10] C：指针与解引用
来源：http://vfo.jqgfzy.top

int *p = &a;  *p = 5;
来源：http://qma.0kj1m.cn

[S11] C：逐行读文件
来源：http://cux.smart0.xyz

FILE *f = fopen("a.txt", "r");
来源：http://apl.zhiwuduotai.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://skv.jyoumei.cn

fclose(f);
来源：http://esd.cucudq.cn

[S12] C：写文件
来源：http://nqq.fktsv.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://exa.zdbjq.cn

[S13] C：宏定义
来源：http://yxl.sweek.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ysd.ywan-chungtsiang.top

[S14] C：枚举
来源：http://gmp.xylfe.cn

enum Color { RED, GREEN, BLUE };
来源：http://glr.zhaomingkeji.xyz

[S15] C：类型转换
来源：http://bbh.nanxinkj.top

(double) a / b
来源：http://zog.ivvv.top

[S16] C：位操作置位
来源：http://biw.ywan-chungtsiang.top

x |= (1 << 3);
来源：http://crs.iojbl.cn

[S17] C：安全拼接字符串
来源：http://erm.jinyuanbaomall.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oum.zhongyouzk.top

[S18] C：命令行参数
来源：http://tkq.zhixingplan.top

int main(int argc, char **argv)
来源：http://ede.zhoulong.xyz

[S19] C：快速排序
来源：http://rnq.shangyingyoupin.top

qsort(a, n, sizeof(int), cmp);
来源：http://tfk.sjlbkw.cn

[S20] C：二分查找
来源：http://ych.gaohongyu789.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vbx.nanxuanxn.top

[S21] C：字符类别判断
来源：http://jyz.sysykeji.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nak.ivvv.top

[S22] C：字符串转数字
来源：http://jbi.yfazqb.com

atoi("42");  strtod("3.14", NULL);
来源：http://xsz.sysykeji.top

[S23] C：随机数
来源：http://dsl.birdmap.top

srand(time(NULL));  int r = rand() % 100;
来源：http://pxt.jlsjyb.cn

[S24] C：获取本地时间
来源：http://ske.dianchejie.cn


<!-- 参考信息 -->