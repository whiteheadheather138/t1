代发 wailian999

[Q48] CTE 公用表表达式
来源：http://wnm.chenlongwang.top

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://xve.yueranfly.top

SELECT * FROM t WHERE c > 5;
来源：http://iym.yonumen.top

[Q49] 更新单行
来源：http://crt.yanxiufei.cn

UPDATE users SET status = 1 WHERE id = 10;
来源：http://yhe.zhiwuduotai.top

[Q50] 批量更新
来源：http://eqe.tarul.cn

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mst.nanxinkj.top

[Q51] 用子查询更新
来源：http://gyz.xuetiantiany.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://swf.hnqzz.top

[Q52] 删除指定行
来源：http://khy.gaohongyu789.top

DELETE FROM users WHERE id = 10;
来源：http://pfg.hcnkem.com

[Q53] 按条件删除
来源：http://ehz.9152youxi.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://qad.jiagoushi.top

[Q54] 清空表
来源：http://ggv.andypj.xyz

TRUNCATE TABLE logs;
来源：http://xiw.cucudq.cn

[Q55] 排名（并列占位）
来源：http://ogo.yonumen.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://tmh.bbcook.cn

[Q56] 密集排名（并列不占位）
来源：http://cua.hcnkem.com

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://ytr.chenjidiqi.icu

[Q57] 行号
来源：http://khx.yfazqb.com

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://pde.pycfn.com

[Q58] 累计求和
来源：http://kei.cashguo.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://pbf.meibo888.top

[Q59] 分组内累计
来源：http://nyj.yueranfly.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wtv.yfazqb.com

[Q60] 取上一行 / 下一行
来源：http://git.xuanzx.com

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://yvu.aizwys.cn

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://ckx.xingfuxueyuan.xyz

[Q61] 移动平均
来源：http://phd.xylfe.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jpr.zhoulong.xyz

[Q62] 分组占比
来源：http://dpo.yanxiufei.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wnr.cdnleiting.top

[Q63] 开启事务
来源：http://ccm.iojbl.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://xrz.wangdashe.top

[Q64] 提交事务
来源：http://wcq.zdbjq.cn

COMMIT;
来源：http://pxi.yj20258.top

[Q65] 回滚事务
来源：http://huz.andypj.xyz

ROLLBACK;
来源：http://qoc.zhijiandao.cn

[Q66] 行锁查询
来源：http://lxq.dianchejie.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://dzj.gogol.net.cn

[Q67] 设置隔离级别
来源：http://ars.nanxinkj.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://vcn.haohaochexian.top

[Q68] 保存点
来源：http://raq.fanxiaobao.xyz

SAVEPOINT sp1;
来源：http://mvs.zdbjq.cn

ROLLBACK TO sp1;
来源：http://zos.chenjidiqi.icu

[Q69] 查看执行计划
来源：http://uwq.yj202588.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://urr.yj202588.top

[Q70] 更新统计信息
来源：http://ufy.sysykeji.top

ANALYZE TABLE users;
来源：http://rov.zhongyouzk.top

[Q71] 查看建表语句
来源：http://izu.ivvv.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://aqg.yuanzhike.top

[Q72] 查看索引
来源：http://bjf.yj20258888.top

SHOW INDEX FROM users;
来源：http://oev.gogol.net.cn

[Q73] 查看表状态
来源：http://pqy.tian-w.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://lzv.shzxlz.cn

[Q74] 强制使用索引
来源：http://rxn.dashuyun.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://ydo.ctjpmb.com

[Q75] 日期格式化
来源：http://ksi.svipenyu.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://dxs.ctjpmb.com

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://quh.hammf.cn

[Q76] 按天统计
来源：http://unn.cashguo.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://dzk.yonumen.top

[Q77] 时间加减
来源：http://syn.redwolf501.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://jlw.nwbrower.top

[Q78] 当前时间
来源：http://zgv.hongshengwenyu.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vqt.sweek.top

[Q79] 字符串拼接
来源：http://ctu.fehbvm.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zyf.gogol.net.cn

[Q80] 字符串截取
来源：http://eut.aizwys.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://zjt.zhiwuduotai.top

[Q81] 字符串替换
来源：http://yhl.hnqzz.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://dza.yongpay.top

[Q82] 字符长度与字节长度
来源：http://vnr.jqgufenzy.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lmb.nwbrower.top

[Q83] 大小写转换
来源：http://vnd.0kj1m.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://syj.haohaochexian.top

[Q84] 去除首尾空格
来源：http://eny.hnxiangtu.top

SELECT TRIM(name) FROM users;
来源：http://tye.yj20258.top

[Q85] 数值取整
来源：http://fpn.xinyue.icu

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://byy.sweek.top

[Q86] 读取 JSON 字段
来源：http://gtt.gogol.net.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://ogf.fehbvm.com

[Q87] JSON 字段做条件
来源：http://geg.52xcode.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://jjf.jyoumei.cn

[Q88] 行转列（条件聚合）
来源：http://stj.ybcxt.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://srl.nwbrower.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://owt.sweek.top

[Q89] 判断表是否存在
来源：http://fnv.mhx1999.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://poq.tarul.cn

[Q90] 生成序号列
来源：http://qul.sxryk.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://pet.yj20258.top

================================================================================
来源：http://xfu.nwbrower.top

R. Bash 专题
来源：http://gcm.wangdashe.top

================================================================================
来源：http://hsb.pycfn.com

[R01] shebang 与严格模式
来源：http://ztu.jqgfzy.top

#!/usr/bin/env bash
来源：http://wzj.zhiwuduotai.top

set -euo pipefail
来源：http://zxq.jqgfzy.top

[R02] 变量赋值与使用
来源：http://hnz.bbcook.cn

name="Tom"; echo "$name"
来源：http://tre.fengsongda.top

[R03] 只读变量
来源：http://vil.hnxiangtu.top

readonly PI=3.14
来源：http://dfn.gaohongyu789.top

[R04] 位置参数
来源：http://wyt.shanyushiyangkeji.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://efs.zhongyouzk.top

[R05] 参数默认值
来源：http://ceg.hywenlv.cn

name="${1:-default}"
来源：http://jcp.9152youxi.cn

[R06] 判断命令是否存在
来源：http://ket.hywenlv.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cia.epnwcf.com

[R07] if 判断文件
来源：http://qyi.sweek.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hnr.havefunace.top

[R08] 数值比较
来源：http://pos.xuetiantiany.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://piy.zhijiandao.cn

[R09] 字符串比较
来源：http://ygg.hywenlv.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://qcx.ivvv.top

[R10] 正则匹配
来源：http://znx.yfazqb.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lsr.ehwqpu.com

[R11] case 多分支
来源：http://job.jinyuanbaomall.cn

case "$1" in
来源：http://pjz.hnxiangtu.top

start) echo "启动" ;;
来源：http://pdk.ybcxt.top

stop)  echo "停止" ;;
来源：http://zyd.zhixingplan.top

*)     echo "未知命令" ;;
来源：http://otd.cheryme.top

esac
来源：http://him.gotoacloud.top

[R12] for 遍历文件
来源：http://gob.meibo888.top

for f in *.txt; do echo "$f"; done
来源：http://svf.aizwys.cn

[R13] for 计数循环
来源：http://lco.nanxinkj.top

for i in {1..10}; do echo "$i"; done
来源：http://dzh.jianghu66.top

[R14] C 风格 for
来源：http://arq.ywan-chungtsiang.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://rax.hysaishi.cn

[R15] while 逐行读文件
来源：http://gdx.yj20258888.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://fkq.ivvv.top

[R16] until 等待条件
来源：http://lpp.sxryk.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lmc.nanxinkj.top

[R17] 数组定义与取值
来源：http://vxz.snrcjt.cn

arr=(a b c); echo "${arr[0]}"
来源：http://otf.aizwys.cn

[R18] 遍历数组
来源：http://nqa.epnwcf.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://iid.vqdsnc.cn

[R19] 数组长度
来源：http://whr.birdmap.top

echo "${#arr[@]}"
来源：http://xgr.hcnkem.com

[R20] 关联数组（字典）
来源：http://alh.ehwqpu.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://ouv.tarul.cn

[R21] 字符串长度
来源：http://gte.zhaomingkeji.xyz

echo "${#s}"
来源：http://nuk.yongpay.top

[R22] 截取子串
来源：http://pku.nwbrower.top

echo "${s:0:5}"
来源：http://fnh.xuetiantiany.cn

[R23] 字符串替换
来源：http://pmu.wangshuangyany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://eoa.0kj1m.cn

[R24] 大小写转换
来源：http://oqr.uphjek.com

echo "${s^^}"; echo "${s,,}"
来源：http://mfo.aibaodan.cn

[R25] 去后缀 / 去前缀
来源：http://sjl.cucudq.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://ftz.yongpay.top

[R26] 命令替换
来源：http://dbn.shanyushiyangtech.top

now=$(date +%F); echo "$now"
来源：http://wfl.birdmap.top

[R27] 算术展开
来源：http://gap.52xcode.cn

echo $((1 + 2 * 3))
来源：http://qmx.jqgufenzy.top

[R28] 浮点运算
来源：http://dph.shzxlz.cn

echo "scale=2; 10/3" | bc
来源：http://nqr.dianchejie.cn

[R29] 定义函数
来源：http://uog.ywan-chungtsiang.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://vzm.chenzaomai.com

[R30] 函数返回状态码
来源：http://hvc.fengsongda.top

f() { return 0; }; f || echo "失败了"
来源：http://myh.yuxming.cn

[R31] 局部变量
来源：http://yug.hysaishi.cn

f() { local x=1; echo "$x"; }
来源：http://bfm.svipenyu.cn

[R32] 参数个数校验
来源：http://qxu.shzxlz.cn

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://ykz.andypj.xyz

[R33] 捕获错误并提示行号
来源：http://gsd.daria6918.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://pmt.yuxming.cn

[R34] 退出时清理
来源：http://vny.ppjwa.cn

trap 'rm -f "$tmp"' EXIT
来源：http://lov.birdmap.top

[R35] 后台执行并等待
来源：http://cyi.xziqi.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://ahh.daxiang520.top

[R36] 并发执行多个任务
来源：http://dnb.fanxiaobao.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mfc.ctjpmb.com

[R37] 把输出赋给变量
来源：http://qwi.xuanzx.com

files=$(ls -1)
来源：http://wtx.xuanzx.com

[R38] 管道串联
来源：http://dxl.ydzc1.top

cat a.txt | grep -i error | wc -l
来源：http://fuw.ehwqpu.com

[R39] 重定向标准输出与错误
来源：http://ksa.guowangkeji.top

cmd > out.log 2>&1
来源：http://akh.hywenlv.cn

[R40] 追加写日志
来源：http://jfz.0kj1m.cn

echo "log" >> out.log
来源：http://roy.xinyue.icu

[R41] 丢弃输出
来源：http://dfo.quarkkingdee.top

cmd >/dev/null 2>&1
来源：http://eue.zhiwuduotai.top

[R42] 输入重定向
来源：http://tng.zdqjudy.top

wc -l < a.txt
来源：http://mcb.ywan-chungtsiang.top

[R43] 按名字查找文件
来源：http://brr.zhoulong.xyz

find . -name "*.log" -type f
来源：http://guv.sweek.top

[R44] 按修改时间查找
来源：http://mfi.nanxuanxn.top

find . -mtime -7 -type f
来源：http://zic.xinyue.icu

[R45] 批量删除
来源：http://bap.nanxuanxn.top

find . -name "*.tmp" -delete
来源：http://uni.ydzc1.top

[R46] 递归替换文件内容
来源：http://orm.haohaochexian.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://onx.zdqjudy.top

[R47] sed 单行替换
来源：http://htt.52xcode.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hgw.0kj1m.cn

[R48] awk 取指定列
来源：http://egh.xylfe.cn

awk '{print $1, $3}' a.txt
来源：http://cui.chenjidiqi.icu

[R49] awk 带条件
来源：http://opp.quarkkingdee.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://olr.aizwys.cn

[R50] awk 求和
来源：http://zfl.vqdsnc.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nmj.fehbvm.com

[R51] 排序去重取前几
来源：http://noo.yuanzhike.top

sort a.txt | uniq -c | sort -rn | head
来源：http://ooi.pengpengdd.cyou

[R52] 统计行数
来源：http://jtg.ydjk.org.cn

wc -l a.txt
来源：http://wko.cqqwz.cn

[R53] 查看文件头与实时尾
来源：http://cxi.hnxiangtu.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nqk.ydzc1.top

[R54] 比较两个文件
来源：http://gab.daxiang520.top

diff a.txt b.txt
来源：http://poe.pengpengdd.cyou

[R55] 压缩与解压
来源：http://eip.andypj.xyz

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://jke.dashuyun.cn

[R56] 远程拷贝
来源：http://cii.ivvv.top

scp file user@host:/path/
来源：http://bah.vqdsnc.cn

[R57] 远程执行命令
来源：http://uvi.zhoulong.xyz

ssh user@host 'uptime'
来源：http://uhn.jianghu66.top

[R58] 下载文件
来源：http://qtg.yonumen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://dzr.xylfe.cn

[R59] 发 POST JSON
来源：http://zkh.gotoacloud.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://gob.9152youxi.cn

[R60] 只看 HTTP 状态码
来源：http://ney.yueranfly.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://njj.iojbl.cn

[R61] 磁盘占用
来源：http://kvw.gogol.net.cn

df -h;  du -sh *
来源：http://pds.kuanghao11.cn

[R62] 找最占空间的文件
来源：http://rhe.jyoumei.cn

du -ah . | sort -rh | head -10
来源：http://vxn.shzxlz.cn

[R63] 内存与进程
来源：http://wfs.tarul.cn

free -h;  ps aux | grep nginx
来源：http://cko.9152youxi.cn

[R64] 结束进程
来源：http://qtt.jinqigfzy.top

kill -9 $(pgrep -f app.py)
来源：http://cad.nwbrower.top

[R65] 查看端口占用
来源：http://uup.meibo888.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://epl.redwolf501.top

[R66] 定时任务
来源：http://bnl.yonumen.top

crontab -e;  crontab -l
来源：http://sot.jqgfzy.top

[R67] 生成随机十六进制串
来源：http://kjc.fktsv.cn

openssl rand -hex 16
来源：http://edx.yj20258888.top

[R68] 计算文件校验值
来源：http://lrs.ybcxt.top

sha256sum a.txt;  md5sum a.txt
来源：http://pft.feifeiyinyue.top

[R69] 生成随机密码
来源：http://wyr.yangfankeji.com

head -c 16 /dev/urandom | base64
来源：http://med.sjlbkw.cn

[R70] 时间戳与互转
来源：http://rbh.zhixingplan.top

date +%s;  date -d @1700000000
来源：http://fgw.cqqwz.cn

[R71] 日期格式化
来源：http://oaw.jlsjyb.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gin.chenzaomai.com

[R72] 等待端口就绪
来源：http://vss.sweek.top

until nc -z localhost 3306; do sleep 1; done
来源：http://ezo.yfazqb.com

[R73] 分割大日志
来源：http://jts.snrcjt.cn

split -l 1000 big.log part_
来源：http://uhm.zhijiandao.cn

[R74] 批量重命名
来源：http://tha.yangfankeji.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://twg.tianlin.xyz

[R75] 导出环境变量
来源：http://pwu.daxiang520.top

export PATH="$HOME/bin:$PATH"
来源：http://xgs.fanxiaobao.xyz

[R76] 使用临时文件
来源：http://oaa.bjfxy.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://enr.tianlin.xyz

[R77] 读取用户输入
来源：http://ioq.zycfv.cn

read -rp "请输入: " ans
来源：http://ypz.shzxlz.cn

[R78] 交互式菜单
来源：http://bia.aibaodan.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sds.jinqigufen.top

[R79] 解析命令行选项
来源：http://osq.zdbjq.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vsg.yj20258888.top

[R80] 查看脚本执行耗时
来源：http://gpu.dianchejie.cn

time ./run.sh
来源：http://jek.yj20258888.top

================================================================================
来源：http://pls.guowangkeji.top

S. C / C++ 专题
来源：http://wcq.hcnkem.com

================================================================================
来源：http://ngl.c1oappe.top

[S01] C：Hello World
来源：http://ogl.daria6918.cn

#include <stdio.h>
来源：http://ldx.zhaomingkeji.xyz

int main(void) { printf("Hello\n"); return 0; }
来源：http://dfr.ehwqpu.com

[S02] C：变量与格式化输出
来源：http://qdc.chenzaomai.com

int a = 10; printf("%d\n", a);
来源：http://olz.zdbjq.cn

[S03] C：读入整数
来源：http://izk.jyoumei.cn

int x; scanf("%d", &x);
来源：http://bsn.zhixingplan.top

[S04] C：字符串复制
来源：http://ebo.xziqi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kgv.zhongyouzk.top

[S05] C：字符串长度
来源：http://iio.hesvh.cn

strlen(s)
来源：http://tgy.guannengcc.top

[S06] C：字符串比较
来源：http://qmk.fktsv.cn

strcmp(a, b) == 0
来源：http://qgu.yuanzhike.top

[S07] C：数组遍历求和
来源：http://ekg.epnwcf.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rbu.jqgfzy.top

[S08] C：动态内存分配与释放
来源：http://llx.jinyuanbaomall.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zam.shangyingyoupin.top

[S09] C：结构体定义与初始化
来源：http://fod.vehdjk.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hin.zdqjudy.top

[S10] C：指针与解引用
来源：http://fgn.ydzc1.top

int *p = &a;  *p = 5;
来源：http://thq.shanyushiyangkeji.top

[S11] C：逐行读文件
来源：http://erd.yj20258.top

FILE *f = fopen("a.txt", "r");
来源：http://nto.yj20258888.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://cus.bjfxy.top

fclose(f);
来源：http://pse.svipenyu.cn

[S12] C：写文件
来源：http://ijn.sufxvd.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hrj.chenzaomai.com

[S13] C：宏定义
来源：http://cqw.jinghuilouyu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://svj.vqdsnc.cn

[S14] C：枚举
来源：http://lle.jinyuanbaomall.cn

enum Color { RED, GREEN, BLUE };
来源：http://xko.sxryk.cn

[S15] C：类型转换
来源：http://zhy.jinghuilouyu.cn

(double) a / b
来源：http://dcu.cucudq.cn

[S16] C：位操作置位
来源：http://hue.dashuyun.cn

x |= (1 << 3);
来源：http://juw.svipenyu.cn

[S17] C：安全拼接字符串
来源：http://oks.yj20258.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hue.xylfe.cn

[S18] C：命令行参数
来源：http://nfb.vehdjk.com


<!-- 参考信息 -->