代发 wailian999

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qum.jinghuilouyu.cn

[Q56] 密集排名（并列不占位）
来源：http://xep.zdbjq.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://nfl.xylfe.cn

[Q57] 行号
来源：http://fxo.yuxming.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://cur.jinqigfzy.top

[Q58] 累计求和
来源：http://mzr.cqqwz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://rxy.ydjk.org.cn

[Q59] 分组内累计
来源：http://ewr.yueranfly.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yjp.jinqigufen.top

[Q60] 取上一行 / 下一行
来源：http://hcw.haohaochexian.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yil.svipenyu.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://edl.xziqi.cn

[Q61] 移动平均
来源：http://fzq.pengpengdd.cyou

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://tdp.yangfankeji.com

[Q62] 分组占比
来源：http://rcu.guannengcc.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ycy.zhijiandao.cn

[Q63] 开启事务
来源：http://edq.andypj.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://foc.xuanzx.com

[Q64] 提交事务
来源：http://gtb.tanke756.top

COMMIT;
来源：http://pli.wangshuangyany.cn

[Q65] 回滚事务
来源：http://kku.pengpengdd.cyou

ROLLBACK;
来源：http://gtc.ydzc1.top

[Q66] 行锁查询
来源：http://ogf.dianchejie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dqt.andypj.xyz

[Q67] 设置隔离级别
来源：http://juh.zhengqikj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://zsz.ybcxt.top

[Q68] 保存点
来源：http://ucb.ywan-chungtsiang.top

SAVEPOINT sp1;
来源：http://qpy.vehdjk.com

ROLLBACK TO sp1;
来源：http://okl.meibo888.top

[Q69] 查看执行计划
来源：http://gqa.nwbrower.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://giu.sufxvd.cn

[Q70] 更新统计信息
来源：http://fnc.jyoumei.cn

ANALYZE TABLE users;
来源：http://gtt.jiagoushi.top

[Q71] 查看建表语句
来源：http://ozm.havefunace.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://ihm.fktsv.cn

[Q72] 查看索引
来源：http://utu.yuanzhike.top

SHOW INDEX FROM users;
来源：http://lea.fktsv.cn

[Q73] 查看表状态
来源：http://rkk.birdmap.top

SHOW TABLE STATUS LIKE 'users';
来源：http://pfv.c1oappe.top

[Q74] 强制使用索引
来源：http://vnn.ppjwa.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://tro.cqqwz.cn

[Q75] 日期格式化
来源：http://knk.zhiwuduotai.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://yyd.shanyushiyangtech.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://qih.chenjidiqi.icu

[Q76] 按天统计
来源：http://rmy.sysykeji.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://ivp.epnwcf.com

[Q77] 时间加减
来源：http://mwy.fzhhl.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://uty.bjfxy.top

[Q78] 当前时间
来源：http://eca.zhijiandao.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://kjv.pengpengdd.cyou

[Q79] 字符串拼接
来源：http://vey.zhoulong.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://uop.316326.xyz

[Q80] 字符串截取
来源：http://xcb.birdmap.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://xca.shangyingyoupin.top

[Q81] 字符串替换
来源：http://yvd.fehbvm.com

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://aou.vqdsnc.cn

[Q82] 字符长度与字节长度
来源：http://kam.hywenlv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ziw.yj202588.top

[Q83] 大小写转换
来源：http://lkn.nwbrower.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hmm.gzhubu.top

[Q84] 去除首尾空格
来源：http://yvt.jianghu66.top

SELECT TRIM(name) FROM users;
来源：http://omc.jyoumei.cn

[Q85] 数值取整
来源：http://fqc.guannengcc.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://owc.tanke756.top

[Q86] 读取 JSON 字段
来源：http://hhm.wangdashe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://uvz.316326.xyz

[Q87] JSON 字段做条件
来源：http://fnn.hcnkem.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jkh.xuanzx.com

[Q88] 行转列（条件聚合）
来源：http://yip.xingfuxueyuan.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kch.cheryme.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mcm.aibaodan.cn

[Q89] 判断表是否存在
来源：http://djl.jinqigfzy.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://nhd.hcnkem.com

[Q90] 生成序号列
来源：http://zkx.gaohongyu789.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hiq.jianghu66.top

================================================================================
来源：http://ybo.shanyushiyangtech.top

R. Bash 专题
来源：http://uph.52xcode.cn

================================================================================
来源：http://uol.ppjwa.cn

[R01] shebang 与严格模式
来源：http://tum.fktsv.cn

#!/usr/bin/env bash
来源：http://cno.0kj1m.cn

set -euo pipefail
来源：http://jos.aibaodan.cn

[R02] 变量赋值与使用
来源：http://wag.cashguo.top

name="Tom"; echo "$name"
来源：http://kax.ppjwa.cn

[R03] 只读变量
来源：http://ndb.tianlin.xyz

readonly PI=3.14
来源：http://twr.kuanghao11.cn

[R04] 位置参数
来源：http://zhb.pycfn.com

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://vuf.c1oappe.top

[R05] 参数默认值
来源：http://dtn.wangshuangyany.cn

name="${1:-default}"
来源：http://arn.bbcook.cn

[R06] 判断命令是否存在
来源：http://xys.sysykeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://rpb.0kj1m.cn

[R07] if 判断文件
来源：http://nyb.ydjk.org.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bfd.bbcook.cn

[R08] 数值比较
来源：http://fyb.fzhhl.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ben.xylfe.cn

[R09] 字符串比较
来源：http://mww.xingfuxueyuan.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://fnh.jinyuanbaomall.cn

[R10] 正则匹配
来源：http://wyr.yj202588.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qpy.yuanzhike.top

[R11] case 多分支
来源：http://mbt.vehdjk.com

case "$1" in
来源：http://tas.hammf.cn

start) echo "启动" ;;
来源：http://klr.zhoulong.xyz

stop)  echo "停止" ;;
来源：http://mjo.hysaishi.cn

*)     echo "未知命令" ;;
来源：http://vkq.wangshuangyany.cn

esac
来源：http://cht.xuanzx.com

[R12] for 遍历文件
来源：http://noj.zhengqikj.top

for f in *.txt; do echo "$f"; done
来源：http://uci.guowangkeji.top

[R13] for 计数循环
来源：http://men.yanxiufei.cn

for i in {1..10}; do echo "$i"; done
来源：http://dar.ivvv.top

[R14] C 风格 for
来源：http://qvl.yj20258888.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://xga.yuanzhike.top

[R15] while 逐行读文件
来源：http://pvu.haohaochexian.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qpt.hnqzz.top

[R16] until 等待条件
来源：http://eau.jinqigfzy.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wfa.dianchejie.cn

[R17] 数组定义与取值
来源：http://bso.zhijiandao.cn

arr=(a b c); echo "${arr[0]}"
来源：http://fjs.yuxming.cn

[R18] 遍历数组
来源：http://kpp.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zml.shangyingyoupin.top

[R19] 数组长度
来源：http://nnf.smart0.xyz

echo "${#arr[@]}"
来源：http://lhm.quarkkingdee.top

[R20] 关联数组（字典）
来源：http://ukh.hcnkem.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://zop.tian-w.cn

[R21] 字符串长度
来源：http://ssx.hnqzz.top

echo "${#s}"
来源：http://yyh.sweek.top

[R22] 截取子串
来源：http://yce.fktsv.cn

echo "${s:0:5}"
来源：http://vls.svipenyu.cn

[R23] 字符串替换
来源：http://vvf.yj202588.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://kad.daria6918.cn

[R24] 大小写转换
来源：http://pst.jyoumei.cn

echo "${s^^}"; echo "${s,,}"
来源：http://jzt.cucudq.cn

[R25] 去后缀 / 去前缀
来源：http://uhz.gaohongyu789.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://brl.epnwcf.com

[R26] 命令替换
来源：http://uvt.hfpthk.cn

now=$(date +%F); echo "$now"
来源：http://wee.ehwqpu.com

[R27] 算术展开
来源：http://lkh.shuidangran.top

echo $((1 + 2 * 3))
来源：http://laa.hywenlv.cn

[R28] 浮点运算
来源：http://ysk.zhengqikj.top

echo "scale=2; 10/3" | bc
来源：http://dlq.yangfankeji.com

[R29] 定义函数
来源：http://lqv.yj20258888.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://bdm.sxryk.cn

[R30] 函数返回状态码
来源：http://edt.jinqigfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://iia.vqdsnc.cn

[R31] 局部变量
来源：http://ava.yuxming.cn

f() { local x=1; echo "$x"; }
来源：http://rhe.sysykeji.top

[R32] 参数个数校验
来源：http://uim.svipenyu.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://its.jqgfzy.top

[R33] 捕获错误并提示行号
来源：http://ich.9152youxi.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ewp.bjfxy.top

[R34] 退出时清理
来源：http://qhu.yangfankeji.com

trap 'rm -f "$tmp"' EXIT
来源：http://uwc.pycfn.com

[R35] 后台执行并等待
来源：http://gxh.tanke756.top

sleep 5 & pid=$!; wait "$pid"
来源：http://vll.zhoulong.xyz

[R36] 并发执行多个任务
来源：http://kag.feifeiyinyue.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://spt.fzhhl.top

[R37] 把输出赋给变量
来源：http://agd.pengpengdd.cyou

files=$(ls -1)
来源：http://vkb.xziqi.cn

[R38] 管道串联
来源：http://bft.yangfankeji.com

cat a.txt | grep -i error | wc -l
来源：http://knw.zhoulong.xyz

[R39] 重定向标准输出与错误
来源：http://rph.yonumen.top

cmd > out.log 2>&1
来源：http://ivs.fanxiaobao.xyz

[R40] 追加写日志
来源：http://wjf.ctjpmb.com

echo "log" >> out.log
来源：http://lgx.gzhubu.top

[R41] 丢弃输出
来源：http://jpg.tarul.cn

cmd >/dev/null 2>&1
来源：http://iox.shanyushiyangkeji.top

[R42] 输入重定向
来源：http://tpt.yuanzhike.top

wc -l < a.txt
来源：http://hhy.haohaochexian.top

[R43] 按名字查找文件
来源：http://shx.hcnkem.com

find . -name "*.log" -type f
来源：http://uyg.redwolf501.top

[R44] 按修改时间查找
来源：http://tfl.vqdsnc.cn

find . -mtime -7 -type f
来源：http://wmr.nanxinkj.top

[R45] 批量删除
来源：http://leh.ydzc1.top

find . -name "*.tmp" -delete
来源：http://paq.jqgufenzy.top

[R46] 递归替换文件内容
来源：http://pis.dianchejie.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qzz.xylfe.cn

[R47] sed 单行替换
来源：http://ttj.yongpay.top

sed -i 's/foo/bar/g' a.txt
来源：http://cmu.andypj.xyz

[R48] awk 取指定列
来源：http://fwt.bjfxy.top

awk '{print $1, $3}' a.txt
来源：http://tpm.fehbvm.com

[R49] awk 带条件
来源：http://zll.bjfxy.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://gvk.redwolf501.top

[R50] awk 求和
来源：http://wcc.nwbrower.top

awk '{s += $2} END {print s}' a.txt
来源：http://fuv.gogol.net.cn

[R51] 排序去重取前几
来源：http://nda.nwbrower.top

sort a.txt | uniq -c | sort -rn | head
来源：http://mnb.quarkkingdee.top

[R52] 统计行数
来源：http://yds.0kj1m.cn

wc -l a.txt
来源：http://rqh.hnxiangtu.top

[R53] 查看文件头与实时尾
来源：http://nmu.xinyue.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://uke.havefunace.top

[R54] 比较两个文件
来源：http://icq.zdqjudy.top

diff a.txt b.txt
来源：http://xty.fanxiaobao.xyz

[R55] 压缩与解压
来源：http://oql.tarul.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wrq.gaohongyu789.top

[R56] 远程拷贝
来源：http://odj.smart0.xyz

scp file user@host:/path/
来源：http://wbr.bjfxy.top

[R57] 远程执行命令
来源：http://ixy.0kj1m.cn

ssh user@host 'uptime'
来源：http://dro.jqgufenzy.top

[R58] 下载文件
来源：http://akz.0kj1m.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://imv.ybcxt.top

[R59] 发 POST JSON
来源：http://jzs.gaohongyu789.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kor.ivvv.top

[R60] 只看 HTTP 状态码
来源：http://pge.9152youxi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pre.hysaishi.cn

[R61] 磁盘占用
来源：http://mtk.sufxvd.cn

df -h;  du -sh *
来源：http://iic.zycfv.cn

[R62] 找最占空间的文件
来源：http://nin.fktsv.cn

du -ah . | sort -rh | head -10
来源：http://wbi.sweek.top

[R63] 内存与进程
来源：http://smd.sweek.top

free -h;  ps aux | grep nginx
来源：http://njf.zhixingplan.top

[R64] 结束进程
来源：http://rmo.dashuyun.cn

kill -9 $(pgrep -f app.py)
来源：http://nnk.pycfn.com

[R65] 查看端口占用
来源：http://qun.sjlbkw.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zct.tanke756.top

[R66] 定时任务
来源：http://fid.cucudq.cn

crontab -e;  crontab -l
来源：http://hiu.jlsjyb.cn

[R67] 生成随机十六进制串
来源：http://ily.gogol.net.cn

openssl rand -hex 16
来源：http://wru.xziqi.cn

[R68] 计算文件校验值
来源：http://nqp.zhongyouzk.top

sha256sum a.txt;  md5sum a.txt
来源：http://xlf.yangfankeji.com

[R69] 生成随机密码
来源：http://yns.yfazqb.com

head -c 16 /dev/urandom | base64
来源：http://zjy.0kj1m.cn

[R70] 时间戳与互转
来源：http://laf.sweek.top

date +%s;  date -d @1700000000
来源：http://qxj.daria6918.cn

[R71] 日期格式化
来源：http://ujy.zhoulong.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://bfa.ivvv.top

[R72] 等待端口就绪
来源：http://rlt.vehdjk.com

until nc -z localhost 3306; do sleep 1; done
来源：http://qch.jqgfzy.top

[R73] 分割大日志
来源：http://vfo.zhoulong.xyz

split -l 1000 big.log part_
来源：http://egu.sxryk.cn

[R74] 批量重命名
来源：http://bvn.feifeiyinyue.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ayb.zdqjudy.top

[R75] 导出环境变量
来源：http://esy.yj20258888.top

export PATH="$HOME/bin:$PATH"
来源：http://tmq.zdbjq.cn

[R76] 使用临时文件
来源：http://gkm.jinghuilouyu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bws.jinqigufen.top

[R77] 读取用户输入
来源：http://nob.yueranfly.top

read -rp "请输入: " ans
来源：http://fro.jiagoushi.top

[R78] 交互式菜单
来源：http://ifc.zhoulong.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://fen.feifeiyinyue.top

[R79] 解析命令行选项
来源：http://jqo.hcnkem.com

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sqj.bbcook.cn

[R80] 查看脚本执行耗时
来源：http://tkp.snrcjt.cn

time ./run.sh
来源：http://mid.cheryme.top

================================================================================
来源：http://ayj.fengsongda.top

S. C / C++ 专题
来源：http://gjn.hnqzz.top

================================================================================
来源：http://vzx.aibaodan.cn

[S01] C：Hello World
来源：http://dhb.pycfn.com

#include <stdio.h>
来源：http://yic.sysykeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wxy.tarul.cn

[S02] C：变量与格式化输出
来源：http://esx.chenzaomai.com

int a = 10; printf("%d\n", a);
来源：http://ybd.sysykeji.top

[S03] C：读入整数
来源：http://mhx.zdbjq.cn

int x; scanf("%d", &x);
来源：http://lbr.fktsv.cn

[S04] C：字符串复制
来源：http://sdl.pycfn.com

char dst[32]; strcpy(dst, "hi");
来源：http://ljk.tanke756.top

[S05] C：字符串长度
来源：http://rwm.tian-w.cn

strlen(s)
来源：http://nyk.svipenyu.cn

[S06] C：字符串比较
来源：http://pms.zhengqikj.top

strcmp(a, b) == 0
来源：http://aks.cdnleiting.top

[S07] C：数组遍历求和
来源：http://ddk.bjfxy.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qia.fktsv.cn

[S08] C：动态内存分配与释放
来源：http://npe.xinyue.icu

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tfc.shangyingyoupin.top

[S09] C：结构体定义与初始化
来源：http://hyj.fehbvm.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kug.yongpay.top

[S10] C：指针与解引用
来源：http://awx.vehdjk.com

int *p = &a;  *p = 5;
来源：http://ami.nwbrower.top

[S11] C：逐行读文件
来源：http://aef.shanyushiyangtech.top

FILE *f = fopen("a.txt", "r");
来源：http://bks.zhoulong.xyz

while (fgets(buf, sizeof buf, f)) { }
来源：http://dwh.ctjpmb.com

fclose(f);
来源：http://kvr.yanxiufei.cn

[S12] C：写文件
来源：http://ykb.chenjidiqi.icu

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pft.shzxlz.cn

[S13] C：宏定义
来源：http://nzu.yuanzhike.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ojv.ywan-chungtsiang.top

[S14] C：枚举
来源：http://qcl.shanyushiyangkeji.top

enum Color { RED, GREEN, BLUE };
来源：http://ukt.yvedp.cn

[S15] C：类型转换
来源：http://cvp.ydzc1.top

(double) a / b
来源：http://cws.meibo888.top

[S16] C：位操作置位
来源：http://kfe.daxiang520.top

x |= (1 << 3);
来源：http://fhd.shanyushiyangkeji.top

[S17] C：安全拼接字符串
来源：http://qke.316326.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jwb.tanke756.top

[S18] C：命令行参数
来源：http://pdp.tanke756.top

int main(int argc, char **argv)
来源：http://mkx.jinyuanbaomall.cn

[S19] C：快速排序
来源：http://aln.ydjk.org.cn

qsort(a, n, sizeof(int), cmp);
来源：http://srm.zhengqikj.top

[S20] C：二分查找
来源：http://hvt.xylfe.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rmg.nanxinkj.top

[S21] C：字符类别判断
来源：http://fnt.tianlin.xyz

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vth.feifeiyinyue.top

[S22] C：字符串转数字
来源：http://mfe.cdnleiting.top

atoi("42");  strtod("3.14", NULL);
来源：http://ihu.havefunace.top

[S23] C：随机数
来源：http://esy.jyoumei.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lqe.yuanzhike.top

[S24] C：获取本地时间
来源：http://dkw.jqgufenzy.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ykx.fanxiaobao.xyz

[S25] C：内存拷贝
来源：http://ini.gotoacloud.top

memcpy(dst, src, n);
来源：http://gvd.chenjidiqi.icu

[S26] C：内存清零
来源：http://mmv.hfpthk.cn


<!-- 参考信息 -->