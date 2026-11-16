代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://nyo.ppjwa.cn

[Q54] 清空表
来源：http://xgc.aibaodan.cn

TRUNCATE TABLE logs;
来源：http://pdc.xziqi.cn

[Q55] 排名（并列占位）
来源：http://vvb.xziqi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zrq.yuxming.cn

[Q56] 密集排名（并列不占位）
来源：http://doj.zhixingplan.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://vhe.tianlin.xyz

[Q57] 行号
来源：http://llw.hnxiangtu.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://qfz.kuanghao11.cn

[Q58] 累计求和
来源：http://gpc.tanke756.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://yoj.redwolf501.top

[Q59] 分组内累计
来源：http://nhx.hysaishi.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://iav.zhongyouzk.top

[Q60] 取上一行 / 下一行
来源：http://mji.zycfv.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mpj.cdnleiting.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://fdu.xinyue.icu

[Q61] 移动平均
来源：http://czt.52xcode.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://bmx.52xcode.cn

[Q62] 分组占比
来源：http://res.epnwcf.com

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ihq.jiagoushi.top

[Q63] 开启事务
来源：http://elc.ctjpmb.com

START TRANSACTION;                -- 或 BEGIN
来源：http://nku.ctjpmb.com

[Q64] 提交事务
来源：http://wks.shanyushiyangkeji.top

COMMIT;
来源：http://dmw.zhongyouzk.top

[Q65] 回滚事务
来源：http://vul.tarul.cn

ROLLBACK;
来源：http://yzb.zdqjudy.top

[Q66] 行锁查询
来源：http://myw.haohaochexian.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://noa.yj202588.top

[Q67] 设置隔离级别
来源：http://xpm.hfpthk.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://huv.shangyingyoupin.top

[Q68] 保存点
来源：http://rra.xuetiantiany.cn

SAVEPOINT sp1;
来源：http://cyt.316326.xyz

ROLLBACK TO sp1;
来源：http://saa.zhengqikj.top

[Q69] 查看执行计划
来源：http://ogf.yuxming.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pxc.kuanghao11.cn

[Q70] 更新统计信息
来源：http://hwv.hongshengwenyu.top

ANALYZE TABLE users;
来源：http://yqq.gzhubu.top

[Q71] 查看建表语句
来源：http://kfq.cucudq.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://vyf.hfpthk.cn

[Q72] 查看索引
来源：http://jmg.chenjidiqi.icu

SHOW INDEX FROM users;
来源：http://bqk.gaohongyu789.top

[Q73] 查看表状态
来源：http://vph.jianghu66.top

SHOW TABLE STATUS LIKE 'users';
来源：http://ibi.epnwcf.com

[Q74] 强制使用索引
来源：http://vws.316326.xyz

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://izi.yfazqb.com

[Q75] 日期格式化
来源：http://rbo.hesvh.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mve.birdmap.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://tlm.sweek.top

[Q76] 按天统计
来源：http://pqc.chenzaomai.com

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dyc.aizwys.cn

[Q77] 时间加减
来源：http://mdx.zdbjq.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qss.fengsongda.top

[Q78] 当前时间
来源：http://yec.yuanzhike.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://ekl.wangdashe.top

[Q79] 字符串拼接
来源：http://fwx.zdqjudy.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uzz.fktsv.cn

[Q80] 字符串截取
来源：http://uhy.xingfuxueyuan.xyz

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bkn.havefunace.top

[Q81] 字符串替换
来源：http://hei.xziqi.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fyx.jqgufenzy.top

[Q82] 字符长度与字节长度
来源：http://bhr.ctjpmb.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://uwb.fanxiaobao.xyz

[Q83] 大小写转换
来源：http://lwl.andypj.xyz

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://rcv.yvedp.cn

[Q84] 去除首尾空格
来源：http://mdv.shanyushiyangkeji.top

SELECT TRIM(name) FROM users;
来源：http://cfp.hesvh.cn

[Q85] 数值取整
来源：http://jbn.yongpay.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://loc.tianlin.xyz

[Q86] 读取 JSON 字段
来源：http://pds.hammf.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://syv.guowangkeji.top

[Q87] JSON 字段做条件
来源：http://hys.iojbl.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jrx.daxiang520.top

[Q88] 行转列（条件聚合）
来源：http://fqv.guowangkeji.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://sqr.wangdashe.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://kld.haohaochexian.top

[Q89] 判断表是否存在
来源：http://pux.ybcxt.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://qbm.havefunace.top

[Q90] 生成序号列
来源：http://djo.guannengcc.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://jvf.xingfuxueyuan.xyz

================================================================================
来源：http://swc.yangfankeji.com

R. Bash 专题
来源：http://iwt.sysykeji.top

================================================================================
来源：http://buw.gzhubu.top

[R01] shebang 与严格模式
来源：http://ghp.tianlin.xyz

#!/usr/bin/env bash
来源：http://cau.ydzc1.top

set -euo pipefail
来源：http://odj.zhaomingkeji.xyz

[R02] 变量赋值与使用
来源：http://ati.mhx1999.top

name="Tom"; echo "$name"
来源：http://sfd.guannengcc.top

[R03] 只读变量
来源：http://fqt.jinqigufen.top

readonly PI=3.14
来源：http://igv.jqgfzy.top

[R04] 位置参数
来源：http://xyh.tian-w.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://dkp.zhixingplan.top

[R05] 参数默认值
来源：http://pre.gogol.net.cn

name="${1:-default}"
来源：http://kps.0kj1m.cn

[R06] 判断命令是否存在
来源：http://vjc.ppjwa.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tbl.yfazqb.com

[R07] if 判断文件
来源：http://rrj.yj20258888.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://elh.316326.xyz

[R08] 数值比较
来源：http://ntk.hfpthk.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://xoq.yonumen.top

[R09] 字符串比较
来源：http://spn.zhoulong.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hnf.hysaishi.cn

[R10] 正则匹配
来源：http://tih.nwbrower.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://gjz.wangdashe.top

[R11] case 多分支
来源：http://bqy.hongshengwenyu.top

case "$1" in
来源：http://hri.shangyingyoupin.top

start) echo "启动" ;;
来源：http://qha.jyoumei.cn

stop)  echo "停止" ;;
来源：http://umz.yj202588.top

*)     echo "未知命令" ;;
来源：http://njc.xylfe.cn

esac
来源：http://zul.fengsongda.top

[R12] for 遍历文件
来源：http://jug.shanyushiyangtech.top

for f in *.txt; do echo "$f"; done
来源：http://llk.xziqi.cn

[R13] for 计数循环
来源：http://qzl.redwolf501.top

for i in {1..10}; do echo "$i"; done
来源：http://yax.sweek.top

[R14] C 风格 for
来源：http://ksr.tianlin.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://zzs.chenzaomai.com

[R15] while 逐行读文件
来源：http://ywj.nanxuanxn.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://eri.dianchejie.cn

[R16] until 等待条件
来源：http://tgo.redwolf501.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hwj.9152youxi.cn

[R17] 数组定义与取值
来源：http://fjr.fktsv.cn

arr=(a b c); echo "${arr[0]}"
来源：http://blm.jinqigufen.top

[R18] 遍历数组
来源：http://bvc.yangfankeji.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://uak.guowangkeji.top

[R19] 数组长度
来源：http://mit.ywan-chungtsiang.top

echo "${#arr[@]}"
来源：http://yfz.zhixingplan.top

[R20] 关联数组（字典）
来源：http://tbk.yueranfly.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://anp.jinqigufen.top

[R21] 字符串长度
来源：http://yqz.wangshuangyany.cn

echo "${#s}"
来源：http://yor.yvedp.cn

[R22] 截取子串
来源：http://zxw.ivvv.top

echo "${s:0:5}"
来源：http://klt.ppjwa.cn

[R23] 字符串替换
来源：http://mtn.pycfn.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://idp.andypj.xyz

[R24] 大小写转换
来源：http://gja.shanyushiyangkeji.top

echo "${s^^}"; echo "${s,,}"
来源：http://zyr.cucudq.cn

[R25] 去后缀 / 去前缀
来源：http://jib.jianghu66.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://gmx.yvedp.cn

[R26] 命令替换
来源：http://vdf.yj20258888.top

now=$(date +%F); echo "$now"
来源：http://fmr.haohaochexian.top

[R27] 算术展开
来源：http://eyt.ctjpmb.com

echo $((1 + 2 * 3))
来源：http://nqm.jianghu66.top

[R28] 浮点运算
来源：http://hbg.gzhubu.top

echo "scale=2; 10/3" | bc
来源：http://vtq.shuidangran.top

[R29] 定义函数
来源：http://axu.uphjek.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://cqi.chenlongwang.top

[R30] 函数返回状态码
来源：http://btw.hfpthk.cn

f() { return 0; }; f || echo "失败了"
来源：http://hay.yvedp.cn

[R31] 局部变量
来源：http://kfe.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://voi.sufxvd.cn

[R32] 参数个数校验
来源：http://rtc.zhongyouzk.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://eoy.shzxlz.cn

[R33] 捕获错误并提示行号
来源：http://ddy.snrcjt.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://qdo.andypj.xyz

[R34] 退出时清理
来源：http://fuv.haohaochexian.top

trap 'rm -f "$tmp"' EXIT
来源：http://zee.xinyue.icu

[R35] 后台执行并等待
来源：http://yzj.feifeiyinyue.top

sleep 5 & pid=$!; wait "$pid"
来源：http://yrk.zdbjq.cn

[R36] 并发执行多个任务
来源：http://slk.hesvh.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://kvf.uphjek.com

[R37] 把输出赋给变量
来源：http://luq.mhx1999.top

files=$(ls -1)
来源：http://btd.vehdjk.com

[R38] 管道串联
来源：http://zmu.hysaishi.cn

cat a.txt | grep -i error | wc -l
来源：http://sue.jinghuilouyu.cn

[R39] 重定向标准输出与错误
来源：http://qdw.fzhhl.top

cmd > out.log 2>&1
来源：http://sqe.smart0.xyz

[R40] 追加写日志
来源：http://lwd.zdbjq.cn

echo "log" >> out.log
来源：http://pkt.zdqjudy.top

[R41] 丢弃输出
来源：http://bmf.9152youxi.cn

cmd >/dev/null 2>&1
来源：http://uaa.yfazqb.com

[R42] 输入重定向
来源：http://bnk.jyoumei.cn

wc -l < a.txt
来源：http://sxh.ctjpmb.com

[R43] 按名字查找文件
来源：http://khh.shzxlz.cn

find . -name "*.log" -type f
来源：http://xkf.bbcook.cn

[R44] 按修改时间查找
来源：http://ewd.jqgfzy.top

find . -mtime -7 -type f
来源：http://wdf.jinghuilouyu.cn

[R45] 批量删除
来源：http://zmi.ppjwa.cn

find . -name "*.tmp" -delete
来源：http://wrk.pengpengdd.cyou

[R46] 递归替换文件内容
来源：http://heb.fktsv.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://aoq.zhengqikj.top

[R47] sed 单行替换
来源：http://tac.zhaomingkeji.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://lmd.yj202588.top

[R48] awk 取指定列
来源：http://szg.hesvh.cn

awk '{print $1, $3}' a.txt
来源：http://etd.vqdsnc.cn

[R49] awk 带条件
来源：http://vwd.hysaishi.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tdg.sysykeji.top

[R50] awk 求和
来源：http://gcf.zhongyouzk.top

awk '{s += $2} END {print s}' a.txt
来源：http://xjx.kuanghao11.cn

[R51] 排序去重取前几
来源：http://jjz.sysykeji.top

sort a.txt | uniq -c | sort -rn | head
来源：http://wno.zhengqikj.top

[R52] 统计行数
来源：http://qeb.ybcxt.top

wc -l a.txt
来源：http://qhq.shanyushiyangkeji.top

[R53] 查看文件头与实时尾
来源：http://kmx.quarkkingdee.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ngy.hcnkem.com

[R54] 比较两个文件
来源：http://bqk.kuanghao11.cn

diff a.txt b.txt
来源：http://htz.sysykeji.top

[R55] 压缩与解压
来源：http://uva.sjlbkw.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sny.shangyingyoupin.top

[R56] 远程拷贝
来源：http://mxh.fanxiaobao.xyz

scp file user@host:/path/
来源：http://snb.birdmap.top

[R57] 远程执行命令
来源：http://jcm.pycfn.com

ssh user@host 'uptime'
来源：http://nuv.zhixingplan.top

[R58] 下载文件
来源：http://gmh.cdnleiting.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kge.hnqzz.top

[R59] 发 POST JSON
来源：http://ain.fengsongda.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cqj.chenzaomai.com

[R60] 只看 HTTP 状态码
来源：http://ifz.wangshuangyany.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://kew.gotoacloud.top

[R61] 磁盘占用
来源：http://mgw.sysykeji.top

df -h;  du -sh *
来源：http://xgd.dianchejie.cn

[R62] 找最占空间的文件
来源：http://ulx.gotoacloud.top

du -ah . | sort -rh | head -10
来源：http://tks.hongshengwenyu.top

[R63] 内存与进程
来源：http://ejq.cdnleiting.top

free -h;  ps aux | grep nginx
来源：http://joz.jinqigufen.top

[R64] 结束进程
来源：http://uau.bjfxy.top

kill -9 $(pgrep -f app.py)
来源：http://wca.daria6918.cn

[R65] 查看端口占用
来源：http://cnx.snrcjt.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sip.yfazqb.com

[R66] 定时任务
来源：http://aua.yvedp.cn

crontab -e;  crontab -l
来源：http://uew.yvedp.cn

[R67] 生成随机十六进制串
来源：http://hwf.zhiwuduotai.top

openssl rand -hex 16
来源：http://lys.nanxinkj.top

[R68] 计算文件校验值
来源：http://ilk.redwolf501.top

sha256sum a.txt;  md5sum a.txt
来源：http://lzm.svipenyu.cn

[R69] 生成随机密码
来源：http://dma.aizwys.cn

head -c 16 /dev/urandom | base64
来源：http://fhy.xylfe.cn

[R70] 时间戳与互转
来源：http://yxq.jiagoushi.top

date +%s;  date -d @1700000000
来源：http://cuj.jyoumei.cn

[R71] 日期格式化
来源：http://eck.mhx1999.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://twt.yj202588.top

[R72] 等待端口就绪
来源：http://nge.xuetiantiany.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jli.shanyushiyangkeji.top

[R73] 分割大日志
来源：http://wzc.cqqwz.cn

split -l 1000 big.log part_
来源：http://dpy.ctjpmb.com

[R74] 批量重命名
来源：http://tur.xziqi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ozc.dianchejie.cn

[R75] 导出环境变量
来源：http://jci.chenzaomai.com

export PATH="$HOME/bin:$PATH"
来源：http://hrv.guowangkeji.top

[R76] 使用临时文件
来源：http://myf.wangdashe.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rfa.nanxuanxn.top

[R77] 读取用户输入
来源：http://glb.snrcjt.cn

read -rp "请输入: " ans
来源：http://dxk.uphjek.com

[R78] 交互式菜单
来源：http://wfv.fanxiaobao.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://qdp.tian-w.cn

[R79] 解析命令行选项
来源：http://big.chenlongwang.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bcx.cheryme.top

[R80] 查看脚本执行耗时
来源：http://qbl.ppjwa.cn

time ./run.sh
来源：http://wll.shuidangran.top

================================================================================
来源：http://zzh.cdnleiting.top

S. C / C++ 专题
来源：http://xei.guowangkeji.top

================================================================================
来源：http://bvv.xziqi.cn

[S01] C：Hello World
来源：http://usi.nwbrower.top

#include <stdio.h>
来源：http://vzz.wangshuangyany.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ntv.zhijiandao.cn

[S02] C：变量与格式化输出
来源：http://fnn.xingfuxueyuan.xyz

int a = 10; printf("%d\n", a);
来源：http://zba.aizwys.cn

[S03] C：读入整数
来源：http://pzl.zdbjq.cn

int x; scanf("%d", &x);
来源：http://blx.pycfn.com

[S04] C：字符串复制
来源：http://zeu.jyoumei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ifo.yangfankeji.com

[S05] C：字符串长度
来源：http://mob.redwolf501.top

strlen(s)
来源：http://xxr.shanyushiyangkeji.top

[S06] C：字符串比较
来源：http://wjn.yuanzhike.top

strcmp(a, b) == 0
来源：http://dgw.jlsjyb.cn

[S07] C：数组遍历求和
来源：http://yfo.fzhhl.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yqj.jqgufenzy.top

[S08] C：动态内存分配与释放
来源：http://hvz.fanxiaobao.xyz

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ole.meibo888.top

[S09] C：结构体定义与初始化
来源：http://ohr.zdqjudy.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tti.xinyue.icu

[S10] C：指针与解引用
来源：http://ewo.zhaomingkeji.xyz

int *p = &a;  *p = 5;
来源：http://kyo.jiagoushi.top

[S11] C：逐行读文件
来源：http://syi.cucudq.cn

FILE *f = fopen("a.txt", "r");
来源：http://bgf.iojbl.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ngn.gogol.net.cn

fclose(f);
来源：http://ooc.epnwcf.com

[S12] C：写文件
来源：http://xxu.hesvh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cwz.yangfankeji.com

[S13] C：宏定义
来源：http://gzt.gogol.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ski.cqqwz.cn

[S14] C：枚举
来源：http://ewn.yonumen.top

enum Color { RED, GREEN, BLUE };
来源：http://fvb.svipenyu.cn

[S15] C：类型转换
来源：http://kkd.jinyuanbaomall.cn

(double) a / b
来源：http://sxw.hnqzz.top

[S16] C：位操作置位
来源：http://cgo.chenjidiqi.icu

x |= (1 << 3);
来源：http://hip.gaohongyu789.top

[S17] C：安全拼接字符串
来源：http://zty.aizwys.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://obp.sufxvd.cn

[S18] C：命令行参数
来源：http://vkt.hysaishi.cn

int main(int argc, char **argv)
来源：http://rxh.tanke756.top

[S19] C：快速排序
来源：http://yrk.feifeiyinyue.top

qsort(a, n, sizeof(int), cmp);
来源：http://khk.zhongyouzk.top

[S20] C：二分查找
来源：http://dcg.svipenyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://max.cdnleiting.top

[S21] C：字符类别判断
来源：http://urd.gzhubu.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://esy.zhaomingkeji.xyz

[S22] C：字符串转数字
来源：http://pbi.xuanzx.com

atoi("42");  strtod("3.14", NULL);
来源：http://hwb.redwolf501.top

[S23] C：随机数
来源：http://dre.jiagoushi.top

srand(time(NULL));  int r = rand() % 100;
来源：http://fxa.zdqjudy.top

[S24] C：获取本地时间
来源：http://bye.hcnkem.com


<!-- 参考信息 -->