代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qkq.xinyue.icu

[Q54] 清空表
来源：http://pig.ybcxt.top

TRUNCATE TABLE logs;
来源：http://hoa.yueranfly.top

[Q55] 排名（并列占位）
来源：http://sgx.zycfv.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vdi.andypj.xyz

[Q56] 密集排名（并列不占位）
来源：http://uap.hysaishi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://obh.xylfe.cn

[Q57] 行号
来源：http://fha.fehbvm.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://aaw.chenjidiqi.icu

[Q58] 累计求和
来源：http://ysf.zhongyouzk.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://lkb.zhiwuduotai.top

[Q59] 分组内累计
来源：http://kvj.xuetiantiany.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ixm.zhaomingkeji.xyz

[Q60] 取上一行 / 下一行
来源：http://ade.sufxvd.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://ink.ybcxt.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://tbg.jinqigfzy.top

[Q61] 移动平均
来源：http://yfd.daxiang520.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yjx.fengsongda.top

[Q62] 分组占比
来源：http://teq.ywan-chungtsiang.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://xnz.cashguo.top

[Q63] 开启事务
来源：http://vch.zhaomingkeji.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://jzx.sxryk.cn

[Q64] 提交事务
来源：http://ynt.yvedp.cn

COMMIT;
来源：http://kfg.xingfuxueyuan.xyz

[Q65] 回滚事务
来源：http://uug.ehwqpu.com

ROLLBACK;
来源：http://qtf.guowangkeji.top

[Q66] 行锁查询
来源：http://kgs.shangyingyoupin.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wgb.shangyingyoupin.top

[Q67] 设置隔离级别
来源：http://zec.chenlongwang.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://szr.xinyue.icu

[Q68] 保存点
来源：http://wsd.shuidangran.top

SAVEPOINT sp1;
来源：http://hgy.hammf.cn

ROLLBACK TO sp1;
来源：http://pzu.aizwys.cn

[Q69] 查看执行计划
来源：http://puc.redwolf501.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://zun.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://utz.xylfe.cn

ANALYZE TABLE users;
来源：http://czq.shangyingyoupin.top

[Q71] 查看建表语句
来源：http://tcb.ppjwa.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://xaj.ehwqpu.com

[Q72] 查看索引
来源：http://mts.xylfe.cn

SHOW INDEX FROM users;
来源：http://qio.wangdashe.top

[Q73] 查看表状态
来源：http://wso.feifeiyinyue.top

SHOW TABLE STATUS LIKE 'users';
来源：http://mte.zhengqikj.top

[Q74] 强制使用索引
来源：http://rdo.wangdashe.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ruw.zhaomingkeji.xyz

[Q75] 日期格式化
来源：http://qko.nanxinkj.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://uqv.shanyushiyangkeji.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ycs.mhx1999.top

[Q76] 按天统计
来源：http://nty.zhijiandao.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://cal.tian-w.cn

[Q77] 时间加减
来源：http://xtp.jinyuanbaomall.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://amn.gotoacloud.top

[Q78] 当前时间
来源：http://pgn.chenjidiqi.icu

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://raq.uphjek.com

[Q79] 字符串拼接
来源：http://dsd.yuanzhike.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://msc.hcnkem.com

[Q80] 字符串截取
来源：http://qxm.xylfe.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://cnz.ehwqpu.com

[Q81] 字符串替换
来源：http://wmy.wangshuangyany.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wuu.jianghu66.top

[Q82] 字符长度与字节长度
来源：http://zbh.sjlbkw.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://zjs.zdbjq.cn

[Q83] 大小写转换
来源：http://vyy.yj20258888.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://yxa.shzxlz.cn

[Q84] 去除首尾空格
来源：http://bns.zhijiandao.cn

SELECT TRIM(name) FROM users;
来源：http://iau.svipenyu.cn

[Q85] 数值取整
来源：http://law.tanke756.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nxx.smart0.xyz

[Q86] 读取 JSON 字段
来源：http://cdz.wangdashe.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hai.hnqzz.top

[Q87] JSON 字段做条件
来源：http://chr.gzhubu.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://oks.chenjidiqi.icu

[Q88] 行转列（条件聚合）
来源：http://yzg.haohaochexian.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mdg.nanxinkj.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://ijm.hfpthk.cn

[Q89] 判断表是否存在
来源：http://yui.dashuyun.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://cwa.tian-w.cn

[Q90] 生成序号列
来源：http://kcq.iojbl.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://phr.cheryme.top

================================================================================
来源：http://uip.zhongyouzk.top

R. Bash 专题
来源：http://dcn.bbcook.cn

================================================================================
来源：http://qni.ydzc1.top

[R01] shebang 与严格模式
来源：http://bah.ctjpmb.com

#!/usr/bin/env bash
来源：http://iwj.hesvh.cn

set -euo pipefail
来源：http://bfs.hysaishi.cn

[R02] 变量赋值与使用
来源：http://sdm.dianchejie.cn

name="Tom"; echo "$name"
来源：http://csj.yfazqb.com

[R03] 只读变量
来源：http://pof.ydjk.org.cn

readonly PI=3.14
来源：http://dwl.jiagoushi.top

[R04] 位置参数
来源：http://vbw.guannengcc.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://srv.yuanzhike.top

[R05] 参数默认值
来源：http://tqb.yj202588.top

name="${1:-default}"
来源：http://okj.cucudq.cn

[R06] 判断命令是否存在
来源：http://srb.tanke756.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://iuv.zhiwuduotai.top

[R07] if 判断文件
来源：http://yfk.316326.xyz

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hfz.wangshuangyany.cn

[R08] 数值比较
来源：http://boz.chenzaomai.com

if (( a > b )); then echo "a 更大"; fi
来源：http://wuz.fzhhl.top

[R09] 字符串比较
来源：http://hmc.zhoulong.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://pnc.jiagoushi.top

[R10] 正则匹配
来源：http://qte.hywenlv.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://sdx.yj20258.top

[R11] case 多分支
来源：http://whh.cashguo.top

case "$1" in
来源：http://qbq.yanxiufei.cn

start) echo "启动" ;;
来源：http://ilp.birdmap.top

stop)  echo "停止" ;;
来源：http://gsy.nanxinkj.top

*)     echo "未知命令" ;;
来源：http://zyy.redwolf501.top

esac
来源：http://dwn.tanke756.top

[R12] for 遍历文件
来源：http://ern.zycfv.cn

for f in *.txt; do echo "$f"; done
来源：http://arr.yuanzhike.top

[R13] for 计数循环
来源：http://rgu.sweek.top

for i in {1..10}; do echo "$i"; done
来源：http://qpc.guannengcc.top

[R14] C 风格 for
来源：http://ayj.guannengcc.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://ebk.wangdashe.top

[R15] while 逐行读文件
来源：http://wzb.guannengcc.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pzd.yuanzhike.top

[R16] until 等待条件
来源：http://bot.jiagoushi.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://tul.xingfuxueyuan.xyz

[R17] 数组定义与取值
来源：http://mii.ivvv.top

arr=(a b c); echo "${arr[0]}"
来源：http://xlc.sweek.top

[R18] 遍历数组
来源：http://wyz.zhixingplan.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fjq.zycfv.cn

[R19] 数组长度
来源：http://xsj.daxiang520.top

echo "${#arr[@]}"
来源：http://npj.jinghuilouyu.cn

[R20] 关联数组（字典）
来源：http://mwg.yj202588.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://gdn.yj20258888.top

[R21] 字符串长度
来源：http://ask.aibaodan.cn

echo "${#s}"
来源：http://taz.ivvv.top

[R22] 截取子串
来源：http://hch.havefunace.top

echo "${s:0:5}"
来源：http://nfj.52xcode.cn

[R23] 字符串替换
来源：http://qig.hnxiangtu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://gcz.fzhhl.top

[R24] 大小写转换
来源：http://iid.hnxiangtu.top

echo "${s^^}"; echo "${s,,}"
来源：http://mvq.tarul.cn

[R25] 去后缀 / 去前缀
来源：http://zbu.birdmap.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://xyg.jinqigufen.top

[R26] 命令替换
来源：http://zjz.tanke756.top

now=$(date +%F); echo "$now"
来源：http://cup.zhaomingkeji.xyz

[R27] 算术展开
来源：http://sdv.ivvv.top

echo $((1 + 2 * 3))
来源：http://kis.yvedp.cn

[R28] 浮点运算
来源：http://aat.zhoulong.xyz

echo "scale=2; 10/3" | bc
来源：http://jhq.jinqigfzy.top

[R29] 定义函数
来源：http://mgd.316326.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ymj.fzhhl.top

[R30] 函数返回状态码
来源：http://ewq.chenzaomai.com

f() { return 0; }; f || echo "失败了"
来源：http://efl.jinghuilouyu.cn

[R31] 局部变量
来源：http://ggj.kuanghao11.cn

f() { local x=1; echo "$x"; }
来源：http://hap.zhiwuduotai.top

[R32] 参数个数校验
来源：http://jau.gaohongyu789.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xbe.daria6918.cn

[R33] 捕获错误并提示行号
来源：http://rnp.jinqigufen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ejy.zhongyouzk.top

[R34] 退出时清理
来源：http://fkg.yj202588.top

trap 'rm -f "$tmp"' EXIT
来源：http://fzv.zhixingplan.top

[R35] 后台执行并等待
来源：http://ygc.hywenlv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://iit.yueranfly.top

[R36] 并发执行多个任务
来源：http://omu.ywan-chungtsiang.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://chh.ybcxt.top

[R37] 把输出赋给变量
来源：http://qbn.fengsongda.top

files=$(ls -1)
来源：http://qtg.yj202588.top

[R38] 管道串联
来源：http://mul.xuanzx.com

cat a.txt | grep -i error | wc -l
来源：http://jvh.cdnleiting.top

[R39] 重定向标准输出与错误
来源：http://hrf.jinqigufen.top

cmd > out.log 2>&1
来源：http://omq.jyoumei.cn

[R40] 追加写日志
来源：http://zvd.guannengcc.top

echo "log" >> out.log
来源：http://zbu.fzhhl.top

[R41] 丢弃输出
来源：http://iog.zhoulong.xyz

cmd >/dev/null 2>&1
来源：http://xcy.andypj.xyz

[R42] 输入重定向
来源：http://kxl.bbcook.cn

wc -l < a.txt
来源：http://hcl.jlsjyb.cn

[R43] 按名字查找文件
来源：http://rip.jinyuanbaomall.cn

find . -name "*.log" -type f
来源：http://ish.wangdashe.top

[R44] 按修改时间查找
来源：http://vej.sxryk.cn

find . -mtime -7 -type f
来源：http://fbc.xylfe.cn

[R45] 批量删除
来源：http://tgq.jqgufenzy.top

find . -name "*.tmp" -delete
来源：http://zhh.redwolf501.top

[R46] 递归替换文件内容
来源：http://ejx.yangfankeji.com

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://fcp.daria6918.cn

[R47] sed 单行替换
来源：http://wgf.gogol.net.cn

sed -i 's/foo/bar/g' a.txt
来源：http://qaq.gaohongyu789.top

[R48] awk 取指定列
来源：http://qzi.shanyushiyangtech.top

awk '{print $1, $3}' a.txt
来源：http://ohq.zhijiandao.cn

[R49] awk 带条件
来源：http://viv.redwolf501.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lyt.ehwqpu.com

[R50] awk 求和
来源：http://iuw.jinqigfzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://dwv.0kj1m.cn

[R51] 排序去重取前几
来源：http://gwr.9152youxi.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://eoh.tianlin.xyz

[R52] 统计行数
来源：http://lub.xingfuxueyuan.xyz

wc -l a.txt
来源：http://rfr.zhaomingkeji.xyz

[R53] 查看文件头与实时尾
来源：http://tol.pycfn.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cre.xinyue.icu

[R54] 比较两个文件
来源：http://kyp.andypj.xyz

diff a.txt b.txt
来源：http://psn.yj20258.top

[R55] 压缩与解压
来源：http://ver.jqgfzy.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lux.jiagoushi.top

[R56] 远程拷贝
来源：http://pqb.hongshengwenyu.top

scp file user@host:/path/
来源：http://dnv.yj20258.top

[R57] 远程执行命令
来源：http://lpx.jiagoushi.top

ssh user@host 'uptime'
来源：http://eut.pycfn.com

[R58] 下载文件
来源：http://fga.aibaodan.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jwy.cheryme.top

[R59] 发 POST JSON
来源：http://xlx.sjlbkw.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gxn.shuidangran.top

[R60] 只看 HTTP 状态码
来源：http://wda.zdbjq.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nhx.dashuyun.cn

[R61] 磁盘占用
来源：http://dlu.cheryme.top

df -h;  du -sh *
来源：http://udi.hnqzz.top

[R62] 找最占空间的文件
来源：http://wnt.chenjidiqi.icu

du -ah . | sort -rh | head -10
来源：http://vxe.bbcook.cn

[R63] 内存与进程
来源：http://mfn.dashuyun.cn

free -h;  ps aux | grep nginx
来源：http://ejr.hammf.cn

[R64] 结束进程
来源：http://kpc.yuanzhike.top

kill -9 $(pgrep -f app.py)
来源：http://cfl.aibaodan.cn

[R65] 查看端口占用
来源：http://fvj.zhaomingkeji.xyz

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qmy.meibo888.top

[R66] 定时任务
来源：http://ykx.dashuyun.cn

crontab -e;  crontab -l
来源：http://tjp.zhijiandao.cn

[R67] 生成随机十六进制串
来源：http://lic.shanyushiyangkeji.top

openssl rand -hex 16
来源：http://nsq.gogol.net.cn

[R68] 计算文件校验值
来源：http://vss.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tij.xuetiantiany.cn

[R69] 生成随机密码
来源：http://wjo.9152youxi.cn

head -c 16 /dev/urandom | base64
来源：http://wqt.shanyushiyangtech.top

[R70] 时间戳与互转
来源：http://cpe.yvedp.cn

date +%s;  date -d @1700000000
来源：http://qtu.yongpay.top

[R71] 日期格式化
来源：http://msx.ivvv.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://kse.aibaodan.cn

[R72] 等待端口就绪
来源：http://dmv.ehwqpu.com

until nc -z localhost 3306; do sleep 1; done
来源：http://cfr.xuanzx.com

[R73] 分割大日志
来源：http://qxd.cashguo.top

split -l 1000 big.log part_
来源：http://xuw.fanxiaobao.xyz

[R74] 批量重命名
来源：http://ccc.epnwcf.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bsn.ppjwa.cn

[R75] 导出环境变量
来源：http://rjx.shangyingyoupin.top

export PATH="$HOME/bin:$PATH"
来源：http://eyg.quarkkingdee.top

[R76] 使用临时文件
来源：http://uxo.dashuyun.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://czk.yj20258888.top

[R77] 读取用户输入
来源：http://bli.wangshuangyany.cn

read -rp "请输入: " ans
来源：http://gfg.zhijiandao.cn

[R78] 交互式菜单
来源：http://tjg.pengpengdd.cyou

select opt in a b c; do echo "$opt"; break; done
来源：http://rzo.zhaomingkeji.xyz

[R79] 解析命令行选项
来源：http://xpq.svipenyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eka.hnxiangtu.top

[R80] 查看脚本执行耗时
来源：http://xez.shanyushiyangtech.top

time ./run.sh
来源：http://woi.yfazqb.com

================================================================================
来源：http://ytp.tianlin.xyz

S. C / C++ 专题
来源：http://yzr.yj20258888.top

================================================================================
来源：http://tvw.yueranfly.top

[S01] C：Hello World
来源：http://uhq.redwolf501.top

#include <stdio.h>
来源：http://myr.tianlin.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://bmi.kuanghao11.cn

[S02] C：变量与格式化输出
来源：http://tes.sweek.top

int a = 10; printf("%d\n", a);
来源：http://gqm.xuetiantiany.cn

[S03] C：读入整数
来源：http://eyw.ydzc1.top

int x; scanf("%d", &x);
来源：http://yxo.fehbvm.com

[S04] C：字符串复制
来源：http://doc.snrcjt.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ojo.pengpengdd.cyou

[S05] C：字符串长度
来源：http://ywj.fengsongda.top

strlen(s)
来源：http://uom.cqqwz.cn

[S06] C：字符串比较
来源：http://kpr.yanxiufei.cn

strcmp(a, b) == 0
来源：http://hag.shzxlz.cn

[S07] C：数组遍历求和
来源：http://vde.nanxinkj.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zmv.jianghu66.top

[S08] C：动态内存分配与释放
来源：http://dvj.aibaodan.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mkn.zhaomingkeji.xyz

[S09] C：结构体定义与初始化
来源：http://dwj.sweek.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bmt.zhaomingkeji.xyz

[S10] C：指针与解引用
来源：http://bhi.xuetiantiany.cn

int *p = &a;  *p = 5;
来源：http://zoc.zhongyouzk.top

[S11] C：逐行读文件
来源：http://dgl.guannengcc.top

FILE *f = fopen("a.txt", "r");
来源：http://vop.daxiang520.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ghk.haohaochexian.top

fclose(f);
来源：http://whc.52xcode.cn

[S12] C：写文件
来源：http://jeb.andypj.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hzt.cdnleiting.top

[S13] C：宏定义
来源：http://xoa.dashuyun.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vad.chenlongwang.top

[S14] C：枚举
来源：http://taq.yonumen.top

enum Color { RED, GREEN, BLUE };
来源：http://hto.hesvh.cn

[S15] C：类型转换
来源：http://rwk.yfazqb.com

(double) a / b
来源：http://zkx.daxiang520.top

[S16] C：位操作置位
来源：http://rol.yfazqb.com

x |= (1 << 3);
来源：http://chm.chenjidiqi.icu

[S17] C：安全拼接字符串
来源：http://gcc.pengpengdd.cyou

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://elz.shanyushiyangtech.top

[S18] C：命令行参数
来源：http://cdj.zhongyouzk.top

int main(int argc, char **argv)
来源：http://kxr.sxryk.cn

[S19] C：快速排序
来源：http://wvo.jqgfzy.top

qsort(a, n, sizeof(int), cmp);
来源：http://hgs.zhixingplan.top

[S20] C：二分查找
来源：http://wjb.mhx1999.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kap.yuanzhike.top

[S21] C：字符类别判断
来源：http://iiv.nanxuanxn.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pfx.fehbvm.com

[S22] C：字符串转数字
来源：http://ijb.yj20258888.top

atoi("42");  strtod("3.14", NULL);
来源：http://hnr.havefunace.top

[S23] C：随机数
来源：http://ooa.yuxming.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qlb.fehbvm.com

[S24] C：获取本地时间
来源：http://fkj.bbcook.cn


<!-- 参考信息 -->