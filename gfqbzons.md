代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://ksh.sweek.top

[Q50] 批量更新
来源：http://avt.fengsongda.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wmr.havefunace.top

[Q51] 用子查询更新
来源：http://ufz.redwolf501.top

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://ymx.0kj1m.cn

[Q52] 删除指定行
来源：http://jhl.jyoumei.cn

DELETE FROM users WHERE id = 10;
来源：http://vey.jinqigufen.top

[Q53] 按条件删除
来源：http://axb.zhengqikj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://fae.zhengqikj.top

[Q54] 清空表
来源：http://fpp.fanxiaobao.xyz

TRUNCATE TABLE logs;
来源：http://byt.hcnkem.com

[Q55] 排名（并列占位）
来源：http://nkm.ppjwa.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://vvo.wangshuangyany.cn

[Q56] 密集排名（并列不占位）
来源：http://mzd.meibo888.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bwe.daxiang520.top

[Q57] 行号
来源：http://rgh.xingfuxueyuan.xyz

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wyo.nanxuanxn.top

[Q58] 累计求和
来源：http://hqj.zhengqikj.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://uhi.jinghuilouyu.cn

[Q59] 分组内累计
来源：http://ily.gzhubu.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://isw.hnxiangtu.top

[Q60] 取上一行 / 下一行
来源：http://pvk.jiagoushi.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://odl.gzhubu.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://soo.xziqi.cn

[Q61] 移动平均
来源：http://lzi.zhengqikj.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://puc.0kj1m.cn

[Q62] 分组占比
来源：http://tof.fengsongda.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://bba.sysykeji.top

[Q63] 开启事务
来源：http://zmj.bjfxy.top

START TRANSACTION;                -- 或 BEGIN
来源：http://njt.chenlongwang.top

[Q64] 提交事务
来源：http://yat.zycfv.cn

COMMIT;
来源：http://lik.tianlin.xyz

[Q65] 回滚事务
来源：http://ank.hongshengwenyu.top

ROLLBACK;
来源：http://czs.cdnleiting.top

[Q66] 行锁查询
来源：http://mtf.tianlin.xyz

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dfa.havefunace.top

[Q67] 设置隔离级别
来源：http://tvt.meibo888.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://kpp.hongshengwenyu.top

[Q68] 保存点
来源：http://nzl.vehdjk.com

SAVEPOINT sp1;
来源：http://fhw.svipenyu.cn

ROLLBACK TO sp1;
来源：http://vwj.hcnkem.com

[Q69] 查看执行计划
来源：http://zvu.hysaishi.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qkf.fzhhl.top

[Q70] 更新统计信息
来源：http://xzy.yongpay.top

ANALYZE TABLE users;
来源：http://yse.hysaishi.cn

[Q71] 查看建表语句
来源：http://cea.xuetiantiany.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://gma.jinqigfzy.top

[Q72] 查看索引
来源：http://dju.bbcook.cn

SHOW INDEX FROM users;
来源：http://vsh.yvedp.cn

[Q73] 查看表状态
来源：http://obt.zhongyouzk.top

SHOW TABLE STATUS LIKE 'users';
来源：http://iww.havefunace.top

[Q74] 强制使用索引
来源：http://ytk.guowangkeji.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://cpw.fanxiaobao.xyz

[Q75] 日期格式化
来源：http://gzg.cqqwz.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hxc.xuetiantiany.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://lbe.fanxiaobao.xyz

[Q76] 按天统计
来源：http://qpq.hongshengwenyu.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mtf.xuanzx.com

[Q77] 时间加减
来源：http://ldi.yanxiufei.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jis.zdbjq.cn

[Q78] 当前时间
来源：http://uhd.daria6918.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://rnx.feifeiyinyue.top

[Q79] 字符串拼接
来源：http://gge.zhoulong.xyz

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://bpj.fengsongda.top

[Q80] 字符串截取
来源：http://wjq.guannengcc.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://yxd.ivvv.top

[Q81] 字符串替换
来源：http://tlq.jinqigfzy.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dni.xingfuxueyuan.xyz

[Q82] 字符长度与字节长度
来源：http://auk.nanxuanxn.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xwk.ydzc1.top

[Q83] 大小写转换
来源：http://evg.ppjwa.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blb.yj20258888.top

[Q84] 去除首尾空格
来源：http://tfn.cdnleiting.top

SELECT TRIM(name) FROM users;
来源：http://qiw.tianlin.xyz

[Q85] 数值取整
来源：http://hat.iojbl.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://gyi.yfazqb.com

[Q86] 读取 JSON 字段
来源：http://hqk.cqqwz.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ywd.chenjidiqi.icu

[Q87] JSON 字段做条件
来源：http://ibh.nanxuanxn.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://ofd.ydjk.org.cn

[Q88] 行转列（条件聚合）
来源：http://pmk.ctjpmb.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://kht.ybcxt.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eww.fktsv.cn

[Q89] 判断表是否存在
来源：http://atc.hongshengwenyu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://rlp.vehdjk.com

[Q90] 生成序号列
来源：http://nrp.jianghu66.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://dfc.xylfe.cn

================================================================================
来源：http://ypr.yueranfly.top

R. Bash 专题
来源：http://lpg.bjfxy.top

================================================================================
来源：http://swt.shanyushiyangtech.top

[R01] shebang 与严格模式
来源：http://cus.hammf.cn

#!/usr/bin/env bash
来源：http://oqx.haohaochexian.top

set -euo pipefail
来源：http://xnn.hywenlv.cn

[R02] 变量赋值与使用
来源：http://uht.dashuyun.cn

name="Tom"; echo "$name"
来源：http://oes.iojbl.cn

[R03] 只读变量
来源：http://zke.havefunace.top

readonly PI=3.14
来源：http://etl.wangdashe.top

[R04] 位置参数
来源：http://nls.zdbjq.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hsb.haohaochexian.top

[R05] 参数默认值
来源：http://ayu.yj20258888.top

name="${1:-default}"
来源：http://gno.hesvh.cn

[R06] 判断命令是否存在
来源：http://sil.ctjpmb.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://quz.xylfe.cn

[R07] if 判断文件
来源：http://xjm.gzhubu.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xpj.quarkkingdee.top

[R08] 数值比较
来源：http://wmk.svipenyu.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://uyx.nanxinkj.top

[R09] 字符串比较
来源：http://pro.smart0.xyz

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zsn.tian-w.cn

[R10] 正则匹配
来源：http://wkz.jinqigufen.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://iim.ivvv.top

[R11] case 多分支
来源：http://vya.yongpay.top

case "$1" in
来源：http://cjg.fktsv.cn

start) echo "启动" ;;
来源：http://ntg.bjfxy.top

stop)  echo "停止" ;;
来源：http://diq.9152youxi.cn

*)     echo "未知命令" ;;
来源：http://hva.hammf.cn

esac
来源：http://tow.daxiang520.top

[R12] for 遍历文件
来源：http://utl.zhiwuduotai.top

for f in *.txt; do echo "$f"; done
来源：http://fkg.yj20258888.top

[R13] for 计数循环
来源：http://gwo.gotoacloud.top

for i in {1..10}; do echo "$i"; done
来源：http://vzv.ydzc1.top

[R14] C 风格 for
来源：http://xoe.yj20258888.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://fiy.jinqigufen.top

[R15] while 逐行读文件
来源：http://hev.hongshengwenyu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://drp.sjlbkw.cn

[R16] until 等待条件
来源：http://vht.jinqigufen.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ile.ivvv.top

[R17] 数组定义与取值
来源：http://kxk.hcnkem.com

arr=(a b c); echo "${arr[0]}"
来源：http://ftr.fengsongda.top

[R18] 遍历数组
来源：http://uih.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ncl.ydjk.org.cn

[R19] 数组长度
来源：http://rcy.redwolf501.top

echo "${#arr[@]}"
来源：http://swn.hammf.cn

[R20] 关联数组（字典）
来源：http://zjt.316326.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://izt.vehdjk.com

[R21] 字符串长度
来源：http://jvl.sjlbkw.cn

echo "${#s}"
来源：http://mzx.zdqjudy.top

[R22] 截取子串
来源：http://qhg.zhijiandao.cn

echo "${s:0:5}"
来源：http://mlw.tanke756.top

[R23] 字符串替换
来源：http://lqg.ppjwa.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ruz.bbcook.cn

[R24] 大小写转换
来源：http://hyt.epnwcf.com

echo "${s^^}"; echo "${s,,}"
来源：http://xcm.andypj.xyz

[R25] 去后缀 / 去前缀
来源：http://erj.tanke756.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://mnq.hfpthk.cn

[R26] 命令替换
来源：http://akm.yvedp.cn

now=$(date +%F); echo "$now"
来源：http://ned.tianlin.xyz

[R27] 算术展开
来源：http://oqx.andypj.xyz

echo $((1 + 2 * 3))
来源：http://vgi.yj20258.top

[R28] 浮点运算
来源：http://don.hywenlv.cn

echo "scale=2; 10/3" | bc
来源：http://pwn.hysaishi.cn

[R29] 定义函数
来源：http://jgi.andypj.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://zpj.yuanzhike.top

[R30] 函数返回状态码
来源：http://igz.gaohongyu789.top

f() { return 0; }; f || echo "失败了"
来源：http://nlo.yangfankeji.com

[R31] 局部变量
来源：http://tht.chenlongwang.top

f() { local x=1; echo "$x"; }
来源：http://eub.daxiang520.top

[R32] 参数个数校验
来源：http://jnn.wangshuangyany.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://can.sweek.top

[R33] 捕获错误并提示行号
来源：http://ttd.jinqigufen.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rwe.xylfe.cn

[R34] 退出时清理
来源：http://vix.jiagoushi.top

trap 'rm -f "$tmp"' EXIT
来源：http://jgs.yueranfly.top

[R35] 后台执行并等待
来源：http://ifb.hysaishi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://xhf.cashguo.top

[R36] 并发执行多个任务
来源：http://paz.guowangkeji.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mfk.ehwqpu.com

[R37] 把输出赋给变量
来源：http://kxt.jinqigufen.top

files=$(ls -1)
来源：http://pmh.zdbjq.cn

[R38] 管道串联
来源：http://yjz.havefunace.top

cat a.txt | grep -i error | wc -l
来源：http://vur.sjlbkw.cn

[R39] 重定向标准输出与错误
来源：http://ygq.nwbrower.top

cmd > out.log 2>&1
来源：http://gec.yj202588.top

[R40] 追加写日志
来源：http://hxz.bbcook.cn

echo "log" >> out.log
来源：http://dlr.yvedp.cn

[R41] 丢弃输出
来源：http://isy.jianghu66.top

cmd >/dev/null 2>&1
来源：http://bgz.ivvv.top

[R42] 输入重定向
来源：http://ddg.gzhubu.top

wc -l < a.txt
来源：http://pth.ctjpmb.com

[R43] 按名字查找文件
来源：http://bgq.yuxming.cn

find . -name "*.log" -type f
来源：http://mwu.yj20258888.top

[R44] 按修改时间查找
来源：http://ifh.fengsongda.top

find . -mtime -7 -type f
来源：http://osm.tarul.cn

[R45] 批量删除
来源：http://bjv.vqdsnc.cn

find . -name "*.tmp" -delete
来源：http://qru.ppjwa.cn

[R46] 递归替换文件内容
来源：http://zja.tian-w.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://rqs.jinyuanbaomall.cn

[R47] sed 单行替换
来源：http://hpz.ydzc1.top

sed -i 's/foo/bar/g' a.txt
来源：http://ggw.hfpthk.cn

[R48] awk 取指定列
来源：http://jwr.yongpay.top

awk '{print $1, $3}' a.txt
来源：http://evs.andypj.xyz

[R49] awk 带条件
来源：http://czp.hammf.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lko.zhixingplan.top

[R50] awk 求和
来源：http://jgu.hywenlv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://pdq.vqdsnc.cn

[R51] 排序去重取前几
来源：http://vff.chenlongwang.top

sort a.txt | uniq -c | sort -rn | head
来源：http://yvn.xuanzx.com

[R52] 统计行数
来源：http://mnn.quarkkingdee.top

wc -l a.txt
来源：http://bfs.haohaochexian.top

[R53] 查看文件头与实时尾
来源：http://srn.fzhhl.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ekt.0kj1m.cn

[R54] 比较两个文件
来源：http://iiw.gzhubu.top

diff a.txt b.txt
来源：http://hqz.havefunace.top

[R55] 压缩与解压
来源：http://qhx.meibo888.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yfp.haohaochexian.top

[R56] 远程拷贝
来源：http://rjw.haohaochexian.top

scp file user@host:/path/
来源：http://vnb.ydzc1.top

[R57] 远程执行命令
来源：http://hzm.jianghu66.top

ssh user@host 'uptime'
来源：http://ogy.mhx1999.top

[R58] 下载文件
来源：http://aia.zycfv.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gya.hysaishi.cn

[R59] 发 POST JSON
来源：http://zuo.redwolf501.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nfv.ctjpmb.com

[R60] 只看 HTTP 状态码
来源：http://bgg.yj20258.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hja.9152youxi.cn

[R61] 磁盘占用
来源：http://pyc.sweek.top

df -h;  du -sh *
来源：http://nwr.tarul.cn

[R62] 找最占空间的文件
来源：http://cau.hcnkem.com

du -ah . | sort -rh | head -10
来源：http://yoe.hysaishi.cn

[R63] 内存与进程
来源：http://ztf.jinyuanbaomall.cn

free -h;  ps aux | grep nginx
来源：http://ebr.xingfuxueyuan.xyz

[R64] 结束进程
来源：http://hxo.xuetiantiany.cn

kill -9 $(pgrep -f app.py)
来源：http://hzf.bjfxy.top

[R65] 查看端口占用
来源：http://yie.pycfn.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://onj.c1oappe.top

[R66] 定时任务
来源：http://bft.vqdsnc.cn

crontab -e;  crontab -l
来源：http://djx.xingfuxueyuan.xyz

[R67] 生成随机十六进制串
来源：http://uoc.quarkkingdee.top

openssl rand -hex 16
来源：http://egm.52xcode.cn

[R68] 计算文件校验值
来源：http://opg.vqdsnc.cn

sha256sum a.txt;  md5sum a.txt
来源：http://tlm.jyoumei.cn

[R69] 生成随机密码
来源：http://sbr.yanxiufei.cn

head -c 16 /dev/urandom | base64
来源：http://bdc.nwbrower.top

[R70] 时间戳与互转
来源：http://mwu.chenzaomai.com

date +%s;  date -d @1700000000
来源：http://esn.chenjidiqi.icu

[R71] 日期格式化
来源：http://irt.yongpay.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://sso.kuanghao11.cn

[R72] 等待端口就绪
来源：http://xfd.fzhhl.top

until nc -z localhost 3306; do sleep 1; done
来源：http://vtz.zhijiandao.cn

[R73] 分割大日志
来源：http://cpj.smart0.xyz

split -l 1000 big.log part_
来源：http://vyz.wangdashe.top

[R74] 批量重命名
来源：http://xpg.iojbl.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qsu.vqdsnc.cn

[R75] 导出环境变量
来源：http://bgh.cdnleiting.top

export PATH="$HOME/bin:$PATH"
来源：http://qlv.tanke756.top

[R76] 使用临时文件
来源：http://uap.xinyue.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hno.yanxiufei.cn

[R77] 读取用户输入
来源：http://uot.svipenyu.cn

read -rp "请输入: " ans
来源：http://unw.52xcode.cn

[R78] 交互式菜单
来源：http://zrw.sxryk.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qgm.yonumen.top

[R79] 解析命令行选项
来源：http://vjr.jinghuilouyu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ehj.ybcxt.top

[R80] 查看脚本执行耗时
来源：http://kxu.shanyushiyangkeji.top

time ./run.sh
来源：http://ybc.quarkkingdee.top

================================================================================
来源：http://xfn.wangdashe.top

S. C / C++ 专题
来源：http://vil.hysaishi.cn

================================================================================
来源：http://xag.guannengcc.top

[S01] C：Hello World
来源：http://tgu.meibo888.top

#include <stdio.h>
来源：http://xba.shanyushiyangkeji.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://wdj.yj202588.top

[S02] C：变量与格式化输出
来源：http://izr.jinyuanbaomall.cn

int a = 10; printf("%d\n", a);
来源：http://tux.meibo888.top

[S03] C：读入整数
来源：http://aqo.ehwqpu.com

int x; scanf("%d", &x);
来源：http://ezy.pengpengdd.cyou

[S04] C：字符串复制
来源：http://lum.xylfe.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vqa.sweek.top

[S05] C：字符串长度
来源：http://ilc.sjlbkw.cn

strlen(s)
来源：http://hoc.pengpengdd.cyou

[S06] C：字符串比较
来源：http://cpz.tanke756.top

strcmp(a, b) == 0
来源：http://roq.0kj1m.cn

[S07] C：数组遍历求和
来源：http://oby.gotoacloud.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fzd.feifeiyinyue.top

[S08] C：动态内存分配与释放
来源：http://frd.aizwys.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xvr.gotoacloud.top

[S09] C：结构体定义与初始化
来源：http://hwb.ydjk.org.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tfw.zdbjq.cn

[S10] C：指针与解引用
来源：http://nvm.chenlongwang.top

int *p = &a;  *p = 5;
来源：http://avc.chenjidiqi.icu

[S11] C：逐行读文件
来源：http://xht.chenzaomai.com

FILE *f = fopen("a.txt", "r");
来源：http://fbi.hywenlv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kwr.316326.xyz

fclose(f);
来源：http://ues.0kj1m.cn

[S12] C：写文件
来源：http://ugg.pengpengdd.cyou

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wbv.guowangkeji.top

[S13] C：宏定义
来源：http://jtq.mhx1999.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://njm.zdqjudy.top

[S14] C：枚举
来源：http://onv.zhongyouzk.top

enum Color { RED, GREEN, BLUE };
来源：http://yvx.ywan-chungtsiang.top

[S15] C：类型转换
来源：http://stq.daxiang520.top

(double) a / b
来源：http://equ.bbcook.cn

[S16] C：位操作置位
来源：http://xap.zhengqikj.top

x |= (1 << 3);
来源：http://xfg.gaohongyu789.top

[S17] C：安全拼接字符串
来源：http://rey.zhaomingkeji.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uky.svipenyu.cn

[S18] C：命令行参数
来源：http://tlq.birdmap.top

int main(int argc, char **argv)
来源：http://mqs.sysykeji.top

[S19] C：快速排序
来源：http://wrm.dianchejie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wnq.ctjpmb.com

[S20] C：二分查找
来源：http://hda.tarul.cn


<!-- 参考信息 -->