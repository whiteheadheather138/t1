代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://att.yuxming.cn

[Q50] 批量更新
来源：http://xgh.yongpay.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wys.yuanzhike.top

[Q51] 用子查询更新
来源：http://yqj.hcnkem.com

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://avb.zdbjq.cn

[Q52] 删除指定行
来源：http://dfx.jinghuilouyu.cn

DELETE FROM users WHERE id = 10;
来源：http://crl.gzhubu.top

[Q53] 按条件删除
来源：http://yzn.zhengqikj.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://gan.ywan-chungtsiang.top

[Q54] 清空表
来源：http://eza.yueranfly.top

TRUNCATE TABLE logs;
来源：http://prp.fanxiaobao.xyz

[Q55] 排名（并列占位）
来源：http://yhe.dianchejie.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://zbj.tanke756.top

[Q56] 密集排名（并列不占位）
来源：http://bwi.c1oappe.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://get.tanke756.top

[Q57] 行号
来源：http://ydt.haohaochexian.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tis.kuanghao11.cn

[Q58] 累计求和
来源：http://tjj.zdqjudy.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://ntu.fengsongda.top

[Q59] 分组内累计
来源：http://hjf.jlsjyb.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://yvi.fehbvm.com

[Q60] 取上一行 / 下一行
来源：http://shy.hnxiangtu.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://gwn.sufxvd.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://sov.shanyushiyangtech.top

[Q61] 移动平均
来源：http://hmy.gzhubu.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://swp.jyoumei.cn

[Q62] 分组占比
来源：http://wgj.wangdashe.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://puz.9152youxi.cn

[Q63] 开启事务
来源：http://zfx.hysaishi.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://nwp.hammf.cn

[Q64] 提交事务
来源：http://jlk.bbcook.cn

COMMIT;
来源：http://bmv.quarkkingdee.top

[Q65] 回滚事务
来源：http://fbn.zhijiandao.cn

ROLLBACK;
来源：http://dzo.sweek.top

[Q66] 行锁查询
来源：http://vhg.shangyingyoupin.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://tjc.bbcook.cn

[Q67] 设置隔离级别
来源：http://voi.yvedp.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://dck.gaohongyu789.top

[Q68] 保存点
来源：http://htp.kuanghao11.cn

SAVEPOINT sp1;
来源：http://vil.yj20258.top

ROLLBACK TO sp1;
来源：http://ncc.zhongyouzk.top

[Q69] 查看执行计划
来源：http://qmo.shangyingyoupin.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://rxc.yangfankeji.com

[Q70] 更新统计信息
来源：http://gzw.sxryk.cn

ANALYZE TABLE users;
来源：http://vde.chenlongwang.top

[Q71] 查看建表语句
来源：http://vmp.9152youxi.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://und.52xcode.cn

[Q72] 查看索引
来源：http://euf.gzhubu.top

SHOW INDEX FROM users;
来源：http://yvy.gotoacloud.top

[Q73] 查看表状态
来源：http://jjg.jianghu66.top

SHOW TABLE STATUS LIKE 'users';
来源：http://cki.hnqzz.top

[Q74] 强制使用索引
来源：http://rwi.yuxming.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ikf.hfpthk.cn

[Q75] 日期格式化
来源：http://guv.tianlin.xyz

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://zcz.hfpthk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://kju.ctjpmb.com

[Q76] 按天统计
来源：http://qmn.xinyue.icu

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://edy.hesvh.cn

[Q77] 时间加减
来源：http://jvv.cashguo.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://rka.fanxiaobao.xyz

[Q78] 当前时间
来源：http://zmn.52xcode.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wbi.shzxlz.cn

[Q79] 字符串拼接
来源：http://qqy.yongpay.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mjn.hysaishi.cn

[Q80] 字符串截取
来源：http://dnc.havefunace.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://ogi.pengpengdd.cyou

[Q81] 字符串替换
来源：http://cuf.zhijiandao.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://jia.xingfuxueyuan.xyz

[Q82] 字符长度与字节长度
来源：http://lcs.jinqigufen.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ojp.jinghuilouyu.cn

[Q83] 大小写转换
来源：http://sfa.yuanzhike.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://ozm.guannengcc.top

[Q84] 去除首尾空格
来源：http://qvw.nanxinkj.top

SELECT TRIM(name) FROM users;
来源：http://hnl.yj20258.top

[Q85] 数值取整
来源：http://bxy.jqgufenzy.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hex.sufxvd.cn

[Q86] 读取 JSON 字段
来源：http://xap.daria6918.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://zyz.xinyue.icu

[Q87] JSON 字段做条件
来源：http://myg.ywan-chungtsiang.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hmn.vqdsnc.cn

[Q88] 行转列（条件聚合）
来源：http://gfi.tianlin.xyz

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://qlr.yfazqb.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://eem.tanke756.top

[Q89] 判断表是否存在
来源：http://fxz.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://uqe.birdmap.top

[Q90] 生成序号列
来源：http://zou.cqqwz.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://iba.xinyue.icu

================================================================================
来源：http://jxk.zhijiandao.cn

R. Bash 专题
来源：http://onn.cdnleiting.top

================================================================================
来源：http://laz.ydzc1.top

[R01] shebang 与严格模式
来源：http://xyr.zdbjq.cn

#!/usr/bin/env bash
来源：http://lol.dianchejie.cn

set -euo pipefail
来源：http://qnr.ppjwa.cn

[R02] 变量赋值与使用
来源：http://qga.316326.xyz

name="Tom"; echo "$name"
来源：http://hks.52xcode.cn

[R03] 只读变量
来源：http://tgf.zhaomingkeji.xyz

readonly PI=3.14
来源：http://thb.cucudq.cn

[R04] 位置参数
来源：http://yli.yj20258888.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yix.fehbvm.com

[R05] 参数默认值
来源：http://tmc.yfazqb.com

name="${1:-default}"
来源：http://dzh.vqdsnc.cn

[R06] 判断命令是否存在
来源：http://rzj.yj202588.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://znw.tanke756.top

[R07] if 判断文件
来源：http://jey.jinghuilouyu.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bsn.nanxinkj.top

[R08] 数值比较
来源：http://ios.cqqwz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://dqc.shangyingyoupin.top

[R09] 字符串比较
来源：http://crw.hfpthk.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://jdf.jiagoushi.top

[R10] 正则匹配
来源：http://mke.fehbvm.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://vur.jinqigufen.top

[R11] case 多分支
来源：http://pcu.iojbl.cn

case "$1" in
来源：http://nvy.sufxvd.cn

start) echo "启动" ;;
来源：http://ehz.ehwqpu.com

stop)  echo "停止" ;;
来源：http://rut.kuanghao11.cn

*)     echo "未知命令" ;;
来源：http://bkp.mhx1999.top

esac
来源：http://xmu.hnqzz.top

[R12] for 遍历文件
来源：http://cuv.hywenlv.cn

for f in *.txt; do echo "$f"; done
来源：http://nvh.sjlbkw.cn

[R13] for 计数循环
来源：http://xps.fehbvm.com

for i in {1..10}; do echo "$i"; done
来源：http://ecg.0kj1m.cn

[R14] C 风格 for
来源：http://ozx.ctjpmb.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://poh.yfazqb.com

[R15] while 逐行读文件
来源：http://fle.tian-w.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mht.ydzc1.top

[R16] until 等待条件
来源：http://enr.yongpay.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://van.epnwcf.com

[R17] 数组定义与取值
来源：http://kys.vqdsnc.cn

arr=(a b c); echo "${arr[0]}"
来源：http://geg.yanxiufei.cn

[R18] 遍历数组
来源：http://avv.jinyuanbaomall.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://vxf.hysaishi.cn

[R19] 数组长度
来源：http://pvy.ybcxt.top

echo "${#arr[@]}"
来源：http://ibm.sufxvd.cn

[R20] 关联数组（字典）
来源：http://ngv.tian-w.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wwx.xylfe.cn

[R21] 字符串长度
来源：http://eao.jinghuilouyu.cn

echo "${#s}"
来源：http://zru.tian-w.cn

[R22] 截取子串
来源：http://vra.aibaodan.cn

echo "${s:0:5}"
来源：http://xrr.daria6918.cn

[R23] 字符串替换
来源：http://kmh.hongshengwenyu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ttb.xingfuxueyuan.xyz

[R24] 大小写转换
来源：http://efu.ppjwa.cn

echo "${s^^}"; echo "${s,,}"
来源：http://xph.gotoacloud.top

[R25] 去后缀 / 去前缀
来源：http://wqs.hysaishi.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://nxi.zdqjudy.top

[R26] 命令替换
来源：http://tpw.chenzaomai.com

now=$(date +%F); echo "$now"
来源：http://elf.yuxming.cn

[R27] 算术展开
来源：http://bhe.yj20258888.top

echo $((1 + 2 * 3))
来源：http://hat.epnwcf.com

[R28] 浮点运算
来源：http://num.cqqwz.cn

echo "scale=2; 10/3" | bc
来源：http://ajf.jqgfzy.top

[R29] 定义函数
来源：http://jsc.hfpthk.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gxi.wangdashe.top

[R30] 函数返回状态码
来源：http://rpf.gotoacloud.top

f() { return 0; }; f || echo "失败了"
来源：http://kfb.shzxlz.cn

[R31] 局部变量
来源：http://vgj.fzhhl.top

f() { local x=1; echo "$x"; }
来源：http://cvu.ehwqpu.com

[R32] 参数个数校验
来源：http://gmv.fktsv.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bci.zhiwuduotai.top

[R33] 捕获错误并提示行号
来源：http://afi.smart0.xyz

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://rjl.ivvv.top

[R34] 退出时清理
来源：http://zsa.yuxming.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dmx.shanyushiyangkeji.top

[R35] 后台执行并等待
来源：http://baw.kuanghao11.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://fny.sufxvd.cn

[R36] 并发执行多个任务
来源：http://jtb.jyoumei.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://uvp.meibo888.top

[R37] 把输出赋给变量
来源：http://yzb.aizwys.cn

files=$(ls -1)
来源：http://guv.jqgfzy.top

[R38] 管道串联
来源：http://rwh.zdbjq.cn

cat a.txt | grep -i error | wc -l
来源：http://khx.pycfn.com

[R39] 重定向标准输出与错误
来源：http://vky.zhiwuduotai.top

cmd > out.log 2>&1
来源：http://guh.snrcjt.cn

[R40] 追加写日志
来源：http://yrx.pycfn.com

echo "log" >> out.log
来源：http://qwt.hnqzz.top

[R41] 丢弃输出
来源：http://cdj.hongshengwenyu.top

cmd >/dev/null 2>&1
来源：http://lug.zhixingplan.top

[R42] 输入重定向
来源：http://vxw.jqgfzy.top

wc -l < a.txt
来源：http://yyy.epnwcf.com

[R43] 按名字查找文件
来源：http://ayw.aizwys.cn

find . -name "*.log" -type f
来源：http://emz.shzxlz.cn

[R44] 按修改时间查找
来源：http://dkl.snrcjt.cn

find . -mtime -7 -type f
来源：http://nyk.zhongyouzk.top

[R45] 批量删除
来源：http://nrx.shuidangran.top

find . -name "*.tmp" -delete
来源：http://ocj.yonumen.top

[R46] 递归替换文件内容
来源：http://oym.shanyushiyangtech.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hxb.gogol.net.cn

[R47] sed 单行替换
来源：http://lyq.jinghuilouyu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://val.cheryme.top

[R48] awk 取指定列
来源：http://uho.yj20258.top

awk '{print $1, $3}' a.txt
来源：http://aqx.sysykeji.top

[R49] awk 带条件
来源：http://eaj.jinghuilouyu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hse.haohaochexian.top

[R50] awk 求和
来源：http://yxt.jqgufenzy.top

awk '{s += $2} END {print s}' a.txt
来源：http://dce.epnwcf.com

[R51] 排序去重取前几
来源：http://gzn.fzhhl.top

sort a.txt | uniq -c | sort -rn | head
来源：http://iea.fanxiaobao.xyz

[R52] 统计行数
来源：http://pdr.fanxiaobao.xyz

wc -l a.txt
来源：http://ahu.yj20258888.top

[R53] 查看文件头与实时尾
来源：http://zbd.chenjidiqi.icu

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mtt.haohaochexian.top

[R54] 比较两个文件
来源：http://off.hcnkem.com

diff a.txt b.txt
来源：http://qvv.quarkkingdee.top

[R55] 压缩与解压
来源：http://wdh.epnwcf.com

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ncp.hfpthk.cn

[R56] 远程拷贝
来源：http://rlx.jqgfzy.top

scp file user@host:/path/
来源：http://fqy.yvedp.cn

[R57] 远程执行命令
来源：http://wls.jiagoushi.top

ssh user@host 'uptime'
来源：http://num.hcnkem.com

[R58] 下载文件
来源：http://xju.shangyingyoupin.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://qtj.hywenlv.cn

[R59] 发 POST JSON
来源：http://obu.316326.xyz

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cil.yonumen.top

[R60] 只看 HTTP 状态码
来源：http://ejg.xuanzx.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jhu.vqdsnc.cn

[R61] 磁盘占用
来源：http://bzv.cheryme.top

df -h;  du -sh *
来源：http://vnd.hnxiangtu.top

[R62] 找最占空间的文件
来源：http://psl.zhoulong.xyz

du -ah . | sort -rh | head -10
来源：http://nfo.yuanzhike.top

[R63] 内存与进程
来源：http://shl.shuidangran.top

free -h;  ps aux | grep nginx
来源：http://hpn.cheryme.top

[R64] 结束进程
来源：http://pze.jyoumei.cn

kill -9 $(pgrep -f app.py)
来源：http://zlj.zycfv.cn

[R65] 查看端口占用
来源：http://jfa.sysykeji.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hat.ctjpmb.com

[R66] 定时任务
来源：http://hvj.316326.xyz

crontab -e;  crontab -l
来源：http://crg.havefunace.top

[R67] 生成随机十六进制串
来源：http://kxl.jlsjyb.cn

openssl rand -hex 16
来源：http://mmn.sjlbkw.cn

[R68] 计算文件校验值
来源：http://jqi.zhijiandao.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yfy.0kj1m.cn

[R69] 生成随机密码
来源：http://tpv.shangyingyoupin.top

head -c 16 /dev/urandom | base64
来源：http://ggy.zhaomingkeji.xyz

[R70] 时间戳与互转
来源：http://rox.iojbl.cn

date +%s;  date -d @1700000000
来源：http://wzr.hywenlv.cn

[R71] 日期格式化
来源：http://zxi.uphjek.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://byn.svipenyu.cn

[R72] 等待端口就绪
来源：http://dvd.hfpthk.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bgw.aibaodan.cn

[R73] 分割大日志
来源：http://klf.fengsongda.top

split -l 1000 big.log part_
来源：http://vrr.zhengqikj.top

[R74] 批量重命名
来源：http://hif.ppjwa.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yen.tianlin.xyz

[R75] 导出环境变量
来源：http://jmr.yongpay.top

export PATH="$HOME/bin:$PATH"
来源：http://pld.xinyue.icu

[R76] 使用临时文件
来源：http://iqw.andypj.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zyl.shzxlz.cn

[R77] 读取用户输入
来源：http://bfc.nanxuanxn.top

read -rp "请输入: " ans
来源：http://ofn.hywenlv.cn

[R78] 交互式菜单
来源：http://goq.jqgfzy.top

select opt in a b c; do echo "$opt"; break; done
来源：http://tex.hammf.cn

[R79] 解析命令行选项
来源：http://ain.zhixingplan.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fkl.jinqigufen.top

[R80] 查看脚本执行耗时
来源：http://tqx.birdmap.top

time ./run.sh
来源：http://ugn.hesvh.cn

================================================================================
来源：http://ihe.xingfuxueyuan.xyz

S. C / C++ 专题
来源：http://kia.shanyushiyangtech.top

================================================================================
来源：http://znp.havefunace.top

[S01] C：Hello World
来源：http://xrc.daria6918.cn

#include <stdio.h>
来源：http://udb.gaohongyu789.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://ghc.xinyue.icu

[S02] C：变量与格式化输出
来源：http://fbg.hesvh.cn

int a = 10; printf("%d\n", a);
来源：http://kmv.zhongyouzk.top

[S03] C：读入整数
来源：http://pwu.sysykeji.top

int x; scanf("%d", &x);
来源：http://rgi.xuetiantiany.cn

[S04] C：字符串复制
来源：http://exu.shanyushiyangkeji.top

char dst[32]; strcpy(dst, "hi");
来源：http://lrd.dashuyun.cn

[S05] C：字符串长度
来源：http://hai.yongpay.top

strlen(s)
来源：http://gmw.hnqzz.top

[S06] C：字符串比较
来源：http://bfq.shzxlz.cn

strcmp(a, b) == 0
来源：http://bci.cqqwz.cn

[S07] C：数组遍历求和
来源：http://yni.shangyingyoupin.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pao.wangshuangyany.cn

[S08] C：动态内存分配与释放
来源：http://unk.nanxuanxn.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mxt.chenlongwang.top

[S09] C：结构体定义与初始化
来源：http://vla.yonumen.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tpb.hnxiangtu.top

[S10] C：指针与解引用
来源：http://xzo.hnqzz.top

int *p = &a;  *p = 5;
来源：http://ftv.nwbrower.top

[S11] C：逐行读文件
来源：http://mqw.dashuyun.cn

FILE *f = fopen("a.txt", "r");
来源：http://qgg.fktsv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ptq.ctjpmb.com

fclose(f);
来源：http://kic.sweek.top

[S12] C：写文件
来源：http://avh.316326.xyz

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hso.shzxlz.cn

[S13] C：宏定义
来源：http://oww.zhongyouzk.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://izw.hfpthk.cn

[S14] C：枚举
来源：http://btf.gogol.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://bmy.jinyuanbaomall.cn

[S15] C：类型转换
来源：http://ire.jinqigufen.top

(double) a / b
来源：http://yhv.mhx1999.top

[S16] C：位操作置位
来源：http://qah.birdmap.top

x |= (1 << 3);
来源：http://aor.chenjidiqi.icu

[S17] C：安全拼接字符串
来源：http://smk.shangyingyoupin.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rot.jinqigfzy.top

[S18] C：命令行参数
来源：http://xej.jinyuanbaomall.cn

int main(int argc, char **argv)
来源：http://afs.shangyingyoupin.top

[S19] C：快速排序
来源：http://awq.wangdashe.top

qsort(a, n, sizeof(int), cmp);
来源：http://lfz.ydjk.org.cn

[S20] C：二分查找
来源：http://hsy.feifeiyinyue.top


<!-- 参考信息 -->