代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wdj.aizwys.cn

[Q50] 批量更新
来源：http://ljm.bjfxy.top

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://pqo.chenjidiqi.icu

[Q51] 用子查询更新
来源：http://frt.snrcjt.cn

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://rxr.hysaishi.cn

[Q52] 删除指定行
来源：http://kvu.jyoumei.cn

DELETE FROM users WHERE id = 10;
来源：http://eal.zhengqikj.top

[Q53] 按条件删除
来源：http://caz.zhixingplan.top

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://zds.yongpay.top

[Q54] 清空表
来源：http://nzc.zhijiandao.cn

TRUNCATE TABLE logs;
来源：http://rui.shangyingyoupin.top

[Q55] 排名（并列占位）
来源：http://qoh.gogol.net.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://bpv.gzhubu.top

[Q56] 密集排名（并列不占位）
来源：http://ham.shanyushiyangkeji.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://smi.shanyushiyangtech.top

[Q57] 行号
来源：http://ath.hfpthk.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://nub.cashguo.top

[Q58] 累计求和
来源：http://eha.ydjk.org.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://vxl.hnqzz.top

[Q59] 分组内累计
来源：http://lbn.hesvh.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://lqm.ywan-chungtsiang.top

[Q60] 取上一行 / 下一行
来源：http://dsa.yanxiufei.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://buo.chenzaomai.com

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xhf.pycfn.com

[Q61] 移动平均
来源：http://byo.9152youxi.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://eml.fktsv.cn

[Q62] 分组占比
来源：http://pnl.haohaochexian.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://swg.quarkkingdee.top

[Q63] 开启事务
来源：http://sku.zhoulong.xyz

START TRANSACTION;                -- 或 BEGIN
来源：http://krs.ivvv.top

[Q64] 提交事务
来源：http://tiw.cucudq.cn

COMMIT;
来源：http://gsa.epnwcf.com

[Q65] 回滚事务
来源：http://bux.nanxuanxn.top

ROLLBACK;
来源：http://zdn.zhixingplan.top

[Q66] 行锁查询
来源：http://aqb.cqqwz.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://nus.yongpay.top

[Q67] 设置隔离级别
来源：http://atl.kuanghao11.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://eei.ppjwa.cn

[Q68] 保存点
来源：http://pfb.c1oappe.top

SAVEPOINT sp1;
来源：http://lho.meibo888.top

ROLLBACK TO sp1;
来源：http://rwh.xingfuxueyuan.xyz

[Q69] 查看执行计划
来源：http://erm.gogol.net.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://yyf.shanyushiyangkeji.top

[Q70] 更新统计信息
来源：http://tgk.haohaochexian.top

ANALYZE TABLE users;
来源：http://pen.zhengqikj.top

[Q71] 查看建表语句
来源：http://hdx.zhongyouzk.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qsi.bbcook.cn

[Q72] 查看索引
来源：http://wtw.bjfxy.top

SHOW INDEX FROM users;
来源：http://sde.chenlongwang.top

[Q73] 查看表状态
来源：http://ghy.pengpengdd.cyou

SHOW TABLE STATUS LIKE 'users';
来源：http://uqt.xylfe.cn

[Q74] 强制使用索引
来源：http://ovd.fehbvm.com

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rva.yuanzhike.top

[Q75] 日期格式化
来源：http://iuc.jqgufenzy.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://ngl.shzxlz.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ylv.feifeiyinyue.top

[Q76] 按天统计
来源：http://gud.fanxiaobao.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://fpy.tanke756.top

[Q77] 时间加减
来源：http://qmz.cheryme.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mwy.shuidangran.top

[Q78] 当前时间
来源：http://ljy.fengsongda.top

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://fes.tanke756.top

[Q79] 字符串拼接
来源：http://vqb.dashuyun.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://cqa.zhiwuduotai.top

[Q80] 字符串截取
来源：http://xhn.sysykeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://bwx.jinghuilouyu.cn

[Q81] 字符串替换
来源：http://dve.chenlongwang.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rud.aizwys.cn

[Q82] 字符长度与字节长度
来源：http://fis.fktsv.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://ukj.wangshuangyany.cn

[Q83] 大小写转换
来源：http://puv.ppjwa.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://cfi.nwbrower.top

[Q84] 去除首尾空格
来源：http://jkv.uphjek.com

SELECT TRIM(name) FROM users;
来源：http://qbj.birdmap.top

[Q85] 数值取整
来源：http://imq.gogol.net.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mcv.jqgufenzy.top

[Q86] 读取 JSON 字段
来源：http://zoj.xuetiantiany.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://dmi.zhoulong.xyz

[Q87] JSON 字段做条件
来源：http://sls.tian-w.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uvs.316326.xyz

[Q88] 行转列（条件聚合）
来源：http://hzf.xinyue.icu

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://xkh.jinghuilouyu.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://sbs.cdnleiting.top

[Q89] 判断表是否存在
来源：http://srl.zhixingplan.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://agf.gzhubu.top

[Q90] 生成序号列
来源：http://kuq.yuanzhike.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mch.sjlbkw.cn

================================================================================
来源：http://enw.jianghu66.top

R. Bash 专题
来源：http://ykv.jqgufenzy.top

================================================================================
来源：http://srr.daria6918.cn

[R01] shebang 与严格模式
来源：http://sep.chenjidiqi.icu

#!/usr/bin/env bash
来源：http://gas.zhijiandao.cn

set -euo pipefail
来源：http://gtf.fehbvm.com

[R02] 变量赋值与使用
来源：http://ukf.xinyue.icu

name="Tom"; echo "$name"
来源：http://nsf.shangyingyoupin.top

[R03] 只读变量
来源：http://fve.yonumen.top

readonly PI=3.14
来源：http://xtn.birdmap.top

[R04] 位置参数
来源：http://ksj.yongpay.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://qcw.andypj.xyz

[R05] 参数默认值
来源：http://pob.cheryme.top

name="${1:-default}"
来源：http://zrh.haohaochexian.top

[R06] 判断命令是否存在
来源：http://tds.fanxiaobao.xyz

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://tcf.hnqzz.top

[R07] if 判断文件
来源：http://hai.yvedp.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://vyw.ehwqpu.com

[R08] 数值比较
来源：http://enb.tarul.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://iiz.shanyushiyangtech.top

[R09] 字符串比较
来源：http://gmz.shanyushiyangtech.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://xix.andypj.xyz

[R10] 正则匹配
来源：http://ump.yanxiufei.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://pnv.zhiwuduotai.top

[R11] case 多分支
来源：http://slu.316326.xyz

case "$1" in
来源：http://vox.tanke756.top

start) echo "启动" ;;
来源：http://jcx.xylfe.cn

stop)  echo "停止" ;;
来源：http://jyu.dianchejie.cn

*)     echo "未知命令" ;;
来源：http://naf.yongpay.top

esac
来源：http://rmn.shanyushiyangkeji.top

[R12] for 遍历文件
来源：http://pqy.pengpengdd.cyou

for f in *.txt; do echo "$f"; done
来源：http://ijx.wangshuangyany.cn

[R13] for 计数循环
来源：http://tab.jianghu66.top

for i in {1..10}; do echo "$i"; done
来源：http://xht.gaohongyu789.top

[R14] C 风格 for
来源：http://iqy.hysaishi.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mvj.svipenyu.cn

[R15] while 逐行读文件
来源：http://wfh.tianlin.xyz

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hds.mhx1999.top

[R16] until 等待条件
来源：http://bma.yj20258.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://ldk.fanxiaobao.xyz

[R17] 数组定义与取值
来源：http://fos.sxryk.cn

arr=(a b c); echo "${arr[0]}"
来源：http://jof.9152youxi.cn

[R18] 遍历数组
来源：http://jjo.ivvv.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://xbh.smart0.xyz

[R19] 数组长度
来源：http://rcf.fanxiaobao.xyz

echo "${#arr[@]}"
来源：http://heo.fehbvm.com

[R20] 关联数组（字典）
来源：http://npq.snrcjt.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://bht.jqgfzy.top

[R21] 字符串长度
来源：http://flc.meibo888.top

echo "${#s}"
来源：http://gix.gzhubu.top

[R22] 截取子串
来源：http://gmn.zhiwuduotai.top

echo "${s:0:5}"
来源：http://vaz.fktsv.cn

[R23] 字符串替换
来源：http://tlv.sweek.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://jjk.zhaomingkeji.xyz

[R24] 大小写转换
来源：http://zlm.316326.xyz

echo "${s^^}"; echo "${s,,}"
来源：http://upn.yj20258888.top

[R25] 去后缀 / 去前缀
来源：http://tlc.jinyuanbaomall.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://rtw.shangyingyoupin.top

[R26] 命令替换
来源：http://bim.sweek.top

now=$(date +%F); echo "$now"
来源：http://fmt.chenzaomai.com

[R27] 算术展开
来源：http://tqs.yuxming.cn

echo $((1 + 2 * 3))
来源：http://mmp.gogol.net.cn

[R28] 浮点运算
来源：http://fra.sxryk.cn

echo "scale=2; 10/3" | bc
来源：http://joj.feifeiyinyue.top

[R29] 定义函数
来源：http://mca.hywenlv.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rbk.316326.xyz

[R30] 函数返回状态码
来源：http://hae.tarul.cn

f() { return 0; }; f || echo "失败了"
来源：http://kbf.xylfe.cn

[R31] 局部变量
来源：http://znb.ehwqpu.com

f() { local x=1; echo "$x"; }
来源：http://vae.ywan-chungtsiang.top

[R32] 参数个数校验
来源：http://muo.fengsongda.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mvv.hnxiangtu.top

[R33] 捕获错误并提示行号
来源：http://ysi.yuxming.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ddm.zhaomingkeji.xyz

[R34] 退出时清理
来源：http://bhv.zhixingplan.top

trap 'rm -f "$tmp"' EXIT
来源：http://lkn.daria6918.cn

[R35] 后台执行并等待
来源：http://nml.hywenlv.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://bnd.shzxlz.cn

[R36] 并发执行多个任务
来源：http://gtj.yuxming.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://prq.yueranfly.top

[R37] 把输出赋给变量
来源：http://eln.316326.xyz

files=$(ls -1)
来源：http://lse.mhx1999.top

[R38] 管道串联
来源：http://vsl.hnqzz.top

cat a.txt | grep -i error | wc -l
来源：http://frs.yfazqb.com

[R39] 重定向标准输出与错误
来源：http://qwy.shangyingyoupin.top

cmd > out.log 2>&1
来源：http://aaf.gogol.net.cn

[R40] 追加写日志
来源：http://vrm.dianchejie.cn

echo "log" >> out.log
来源：http://tep.nanxuanxn.top

[R41] 丢弃输出
来源：http://nmu.hywenlv.cn

cmd >/dev/null 2>&1
来源：http://dxq.yj20258888.top

[R42] 输入重定向
来源：http://rog.vehdjk.com

wc -l < a.txt
来源：http://znv.jqgufenzy.top

[R43] 按名字查找文件
来源：http://zup.jyoumei.cn

find . -name "*.log" -type f
来源：http://doo.tarul.cn

[R44] 按修改时间查找
来源：http://vli.xuanzx.com

find . -mtime -7 -type f
来源：http://xhl.shangyingyoupin.top

[R45] 批量删除
来源：http://tib.yvedp.cn

find . -name "*.tmp" -delete
来源：http://bjj.xziqi.cn

[R46] 递归替换文件内容
来源：http://duq.yvedp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ifm.zhijiandao.cn

[R47] sed 单行替换
来源：http://sxa.hongshengwenyu.top

sed -i 's/foo/bar/g' a.txt
来源：http://xen.jqgufenzy.top

[R48] awk 取指定列
来源：http://kwx.zdqjudy.top

awk '{print $1, $3}' a.txt
来源：http://pmr.tanke756.top

[R49] awk 带条件
来源：http://uyz.52xcode.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yfv.yfazqb.com

[R50] awk 求和
来源：http://zur.zycfv.cn

awk '{s += $2} END {print s}' a.txt
来源：http://xwt.zhiwuduotai.top

[R51] 排序去重取前几
来源：http://wxu.xingfuxueyuan.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://diq.jlsjyb.cn

[R52] 统计行数
来源：http://bur.jyoumei.cn

wc -l a.txt
来源：http://ffm.feifeiyinyue.top

[R53] 查看文件头与实时尾
来源：http://rwf.svipenyu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cqn.zhiwuduotai.top

[R54] 比较两个文件
来源：http://abk.aibaodan.cn

diff a.txt b.txt
来源：http://ihg.cashguo.top

[R55] 压缩与解压
来源：http://adt.ydzc1.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rtv.meibo888.top

[R56] 远程拷贝
来源：http://mbz.shzxlz.cn

scp file user@host:/path/
来源：http://vfe.wangdashe.top

[R57] 远程执行命令
来源：http://cwq.yj20258888.top

ssh user@host 'uptime'
来源：http://vkx.nanxinkj.top

[R58] 下载文件
来源：http://dhm.shangyingyoupin.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://rbi.xinyue.icu

[R59] 发 POST JSON
来源：http://pfz.wangshuangyany.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://puu.xingfuxueyuan.xyz

[R60] 只看 HTTP 状态码
来源：http://ard.ctjpmb.com

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sgc.zhoulong.xyz

[R61] 磁盘占用
来源：http://tiy.gaohongyu789.top

df -h;  du -sh *
来源：http://rrw.shuidangran.top

[R62] 找最占空间的文件
来源：http://tpe.jqgfzy.top

du -ah . | sort -rh | head -10
来源：http://fat.zdbjq.cn

[R63] 内存与进程
来源：http://kky.aizwys.cn

free -h;  ps aux | grep nginx
来源：http://apf.yj202588.top

[R64] 结束进程
来源：http://okv.shuidangran.top

kill -9 $(pgrep -f app.py)
来源：http://mmi.chenlongwang.top

[R65] 查看端口占用
来源：http://tda.hammf.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://pxc.xylfe.cn

[R66] 定时任务
来源：http://udo.zhongyouzk.top

crontab -e;  crontab -l
来源：http://lkz.jianghu66.top

[R67] 生成随机十六进制串
来源：http://zay.xziqi.cn

openssl rand -hex 16
来源：http://emm.0kj1m.cn

[R68] 计算文件校验值
来源：http://bzf.jiagoushi.top

sha256sum a.txt;  md5sum a.txt
来源：http://ams.cdnleiting.top

[R69] 生成随机密码
来源：http://kcc.ctjpmb.com

head -c 16 /dev/urandom | base64
来源：http://oyx.tianlin.xyz

[R70] 时间戳与互转
来源：http://wnr.fanxiaobao.xyz

date +%s;  date -d @1700000000
来源：http://bhu.0kj1m.cn

[R71] 日期格式化
来源：http://cpr.pycfn.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://qxp.jinghuilouyu.cn

[R72] 等待端口就绪
来源：http://vqw.xuanzx.com

until nc -z localhost 3306; do sleep 1; done
来源：http://yzl.aizwys.cn

[R73] 分割大日志
来源：http://ehz.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://yzj.hcnkem.com

[R74] 批量重命名
来源：http://jvb.fehbvm.com

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://yiu.0kj1m.cn

[R75] 导出环境变量
来源：http://lib.sweek.top

export PATH="$HOME/bin:$PATH"
来源：http://uip.fehbvm.com

[R76] 使用临时文件
来源：http://onq.guannengcc.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mij.yvedp.cn

[R77] 读取用户输入
来源：http://vli.kuanghao11.cn

read -rp "请输入: " ans
来源：http://fpo.yj202588.top

[R78] 交互式菜单
来源：http://tgs.zhoulong.xyz

select opt in a b c; do echo "$opt"; break; done
来源：http://pxu.cashguo.top

[R79] 解析命令行选项
来源：http://cmu.fengsongda.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oem.birdmap.top

[R80] 查看脚本执行耗时
来源：http://hpk.shanyushiyangtech.top

time ./run.sh
来源：http://prg.hfpthk.cn

================================================================================
来源：http://iqh.andypj.xyz

S. C / C++ 专题
来源：http://brj.yj20258888.top

================================================================================
来源：http://otd.fktsv.cn

[S01] C：Hello World
来源：http://ygt.zhiwuduotai.top

#include <stdio.h>
来源：http://tvt.jinqigufen.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://lwo.jyoumei.cn

[S02] C：变量与格式化输出
来源：http://uja.zhongyouzk.top

int a = 10; printf("%d\n", a);
来源：http://cvn.9152youxi.cn

[S03] C：读入整数
来源：http://ksc.svipenyu.cn

int x; scanf("%d", &x);
来源：http://yhs.hnqzz.top

[S04] C：字符串复制
来源：http://hep.cdnleiting.top

char dst[32]; strcpy(dst, "hi");
来源：http://mjd.hesvh.cn

[S05] C：字符串长度
来源：http://net.c1oappe.top

strlen(s)
来源：http://mnu.nanxuanxn.top

[S06] C：字符串比较
来源：http://vee.yueranfly.top

strcmp(a, b) == 0
来源：http://xyq.tianlin.xyz

[S07] C：数组遍历求和
来源：http://aam.hesvh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fjd.cdnleiting.top

[S08] C：动态内存分配与释放
来源：http://oze.yonumen.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gbc.zdbjq.cn

[S09] C：结构体定义与初始化
来源：http://hll.haohaochexian.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bqt.yj20258888.top

[S10] C：指针与解引用
来源：http://xdr.sweek.top

int *p = &a;  *p = 5;
来源：http://xsb.shzxlz.cn

[S11] C：逐行读文件
来源：http://clj.uphjek.com

FILE *f = fopen("a.txt", "r");
来源：http://emp.sxryk.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nuk.tianlin.xyz

fclose(f);
来源：http://pgm.hcnkem.com

[S12] C：写文件
来源：http://vfc.gogol.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://syg.ppjwa.cn

[S13] C：宏定义
来源：http://fzh.jyoumei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vmv.yanxiufei.cn

[S14] C：枚举
来源：http://uxh.yonumen.top

enum Color { RED, GREEN, BLUE };
来源：http://hpe.wangdashe.top

[S15] C：类型转换
来源：http://yzn.pycfn.com

(double) a / b
来源：http://omo.zhongyouzk.top

[S16] C：位操作置位
来源：http://suw.ppjwa.cn

x |= (1 << 3);
来源：http://mif.gaohongyu789.top

[S17] C：安全拼接字符串
来源：http://ddf.sweek.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eyd.ydjk.org.cn

[S18] C：命令行参数
来源：http://nqk.hnxiangtu.top

int main(int argc, char **argv)
来源：http://ybc.xziqi.cn

[S19] C：快速排序
来源：http://aoz.chenjidiqi.icu

qsort(a, n, sizeof(int), cmp);
来源：http://euu.sjlbkw.cn

[S20] C：二分查找
来源：http://zrq.yueranfly.top


<!-- 参考信息 -->