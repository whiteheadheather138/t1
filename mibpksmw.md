代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://lxn.hammf.cn

[Q52] 删除指定行
来源：http://keh.yuxming.cn

DELETE FROM users WHERE id = 10;
来源：http://geu.jianghu66.top

[Q53] 按条件删除
来源：http://poz.xuetiantiany.cn

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://dhs.shangyingyoupin.top

[Q54] 清空表
来源：http://kfz.shanyushiyangtech.top

TRUNCATE TABLE logs;
来源：http://naw.gogol.net.cn

[Q55] 排名（并列占位）
来源：http://ztl.9152youxi.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://osy.aibaodan.cn

[Q56] 密集排名（并列不占位）
来源：http://fjc.xuetiantiany.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bhe.meibo888.top

[Q57] 行号
来源：http://rve.jinqigfzy.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hqp.smart0.xyz

[Q58] 累计求和
来源：http://oaw.sysykeji.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://dwp.yj20258888.top

[Q59] 分组内累计
来源：http://lps.bjfxy.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ffi.xuetiantiany.cn

[Q60] 取上一行 / 下一行
来源：http://tdp.nanxinkj.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://imw.wangdashe.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://xuc.pycfn.com

[Q61] 移动平均
来源：http://swm.hnqzz.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mkz.yj20258888.top

[Q62] 分组占比
来源：http://imp.smart0.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ajd.fengsongda.top

[Q63] 开启事务
来源：http://qft.shanyushiyangkeji.top

START TRANSACTION;                -- 或 BEGIN
来源：http://rwf.xinyue.icu

[Q64] 提交事务
来源：http://vhd.52xcode.cn

COMMIT;
来源：http://rbt.ydjk.org.cn

[Q65] 回滚事务
来源：http://fgz.shangyingyoupin.top

ROLLBACK;
来源：http://fpq.quarkkingdee.top

[Q66] 行锁查询
来源：http://urw.snrcjt.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ogi.vqdsnc.cn

[Q67] 设置隔离级别
来源：http://gdt.haohaochexian.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wwn.xingfuxueyuan.xyz

[Q68] 保存点
来源：http://pjc.quarkkingdee.top

SAVEPOINT sp1;
来源：http://zba.hywenlv.cn

ROLLBACK TO sp1;
来源：http://dsr.fanxiaobao.xyz

[Q69] 查看执行计划
来源：http://pyq.jinqigfzy.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://vdq.hysaishi.cn

[Q70] 更新统计信息
来源：http://ufq.xinyue.icu

ANALYZE TABLE users;
来源：http://wvs.hysaishi.cn

[Q71] 查看建表语句
来源：http://gjk.gotoacloud.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://scv.xylfe.cn

[Q72] 查看索引
来源：http://loe.cheryme.top

SHOW INDEX FROM users;
来源：http://ohm.cheryme.top

[Q73] 查看表状态
来源：http://pvy.hywenlv.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://cba.gotoacloud.top

[Q74] 强制使用索引
来源：http://bsi.yongpay.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://rti.pycfn.com

[Q75] 日期格式化
来源：http://fvm.tian-w.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nmt.birdmap.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://eme.dianchejie.cn

[Q76] 按天统计
来源：http://mcd.shangyingyoupin.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://zuz.nwbrower.top

[Q77] 时间加减
来源：http://ltc.52xcode.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://evf.jqgfzy.top

[Q78] 当前时间
来源：http://myy.0kj1m.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vzd.zhongyouzk.top

[Q79] 字符串拼接
来源：http://vhc.jinqigufen.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hwd.redwolf501.top

[Q80] 字符串截取
来源：http://cnf.c1oappe.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://jnt.bjfxy.top

[Q81] 字符串替换
来源：http://tat.wangdashe.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://ggr.hnxiangtu.top

[Q82] 字符长度与字节长度
来源：http://eno.aibaodan.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://lnb.sxryk.cn

[Q83] 大小写转换
来源：http://obv.hfpthk.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://qlh.xylfe.cn

[Q84] 去除首尾空格
来源：http://cce.yongpay.top

SELECT TRIM(name) FROM users;
来源：http://zru.meibo888.top

[Q85] 数值取整
来源：http://qlb.c1oappe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nig.jinqigfzy.top

[Q86] 读取 JSON 字段
来源：http://rde.yvedp.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://spj.yvedp.cn

[Q87] JSON 字段做条件
来源：http://nkc.jyoumei.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://nmo.yanxiufei.cn

[Q88] 行转列（条件聚合）
来源：http://dzu.epnwcf.com

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://rcr.jqgfzy.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hdr.cqqwz.cn

[Q89] 判断表是否存在
来源：http://wev.0kj1m.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://imf.andypj.xyz

[Q90] 生成序号列
来源：http://ftd.zhoulong.xyz

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://taq.zhongyouzk.top

================================================================================
来源：http://lez.gogol.net.cn

R. Bash 专题
来源：http://kod.0kj1m.cn

================================================================================
来源：http://kvg.c1oappe.top

[R01] shebang 与严格模式
来源：http://fwp.shanyushiyangkeji.top

#!/usr/bin/env bash
来源：http://qpx.fktsv.cn

set -euo pipefail
来源：http://mfg.xingfuxueyuan.xyz

[R02] 变量赋值与使用
来源：http://cca.sysykeji.top

name="Tom"; echo "$name"
来源：http://npy.yuanzhike.top

[R03] 只读变量
来源：http://hzn.guannengcc.top

readonly PI=3.14
来源：http://ccx.zhiwuduotai.top

[R04] 位置参数
来源：http://oex.52xcode.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://cfn.hysaishi.cn

[R05] 参数默认值
来源：http://ifs.jinqigufen.top

name="${1:-default}"
来源：http://lii.xuetiantiany.cn

[R06] 判断命令是否存在
来源：http://aqz.nwbrower.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ywl.316326.xyz

[R07] if 判断文件
来源：http://qge.0kj1m.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://ltg.zycfv.cn

[R08] 数值比较
来源：http://bbi.hesvh.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://hxm.9152youxi.cn

[R09] 字符串比较
来源：http://svq.52xcode.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://kcy.zhixingplan.top

[R10] 正则匹配
来源：http://lbh.sweek.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://zcj.shanyushiyangtech.top

[R11] case 多分支
来源：http://qzx.cdnleiting.top

case "$1" in
来源：http://jhm.yanxiufei.cn

start) echo "启动" ;;
来源：http://hfd.pengpengdd.cyou

stop)  echo "停止" ;;
来源：http://jti.fehbvm.com

*)     echo "未知命令" ;;
来源：http://ndv.gzhubu.top

esac
来源：http://hgf.hywenlv.cn

[R12] for 遍历文件
来源：http://hks.xylfe.cn

for f in *.txt; do echo "$f"; done
来源：http://jso.0kj1m.cn

[R13] for 计数循环
来源：http://jgt.hongshengwenyu.top

for i in {1..10}; do echo "$i"; done
来源：http://iuv.jinghuilouyu.cn

[R14] C 风格 for
来源：http://odm.daria6918.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://avw.wangdashe.top

[R15] while 逐行读文件
来源：http://dap.fktsv.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://qjy.52xcode.cn

[R16] until 等待条件
来源：http://tax.sjlbkw.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://huz.shuidangran.top

[R17] 数组定义与取值
来源：http://hxd.sysykeji.top

arr=(a b c); echo "${arr[0]}"
来源：http://okf.fktsv.cn

[R18] 遍历数组
来源：http://sni.hammf.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oui.svipenyu.cn

[R19] 数组长度
来源：http://peh.jyoumei.cn

echo "${#arr[@]}"
来源：http://cia.gzhubu.top

[R20] 关联数组（字典）
来源：http://wos.jinghuilouyu.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qms.fehbvm.com

[R21] 字符串长度
来源：http://qoy.chenlongwang.top

echo "${#s}"
来源：http://ddu.bjfxy.top

[R22] 截取子串
来源：http://guw.jinghuilouyu.cn

echo "${s:0:5}"
来源：http://fne.birdmap.top

[R23] 字符串替换
来源：http://ohb.xylfe.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://knt.snrcjt.cn

[R24] 大小写转换
来源：http://kee.jiagoushi.top

echo "${s^^}"; echo "${s,,}"
来源：http://lzj.hfpthk.cn

[R25] 去后缀 / 去前缀
来源：http://mgo.xuanzx.com

echo "${f%.txt}"; echo "${f#./}"
来源：http://msk.xuetiantiany.cn

[R26] 命令替换
来源：http://eee.yonumen.top

now=$(date +%F); echo "$now"
来源：http://zql.ctjpmb.com

[R27] 算术展开
来源：http://nco.yj20258888.top

echo $((1 + 2 * 3))
来源：http://tfs.ppjwa.cn

[R28] 浮点运算
来源：http://fmo.cashguo.top

echo "scale=2; 10/3" | bc
来源：http://nit.gaohongyu789.top

[R29] 定义函数
来源：http://hqi.cqqwz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://nal.tarul.cn

[R30] 函数返回状态码
来源：http://qqz.cqqwz.cn

f() { return 0; }; f || echo "失败了"
来源：http://fta.zhixingplan.top

[R31] 局部变量
来源：http://cxt.daxiang520.top

f() { local x=1; echo "$x"; }
来源：http://iif.ydzc1.top

[R32] 参数个数校验
来源：http://wvf.zhengqikj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://fmf.yj20258888.top

[R33] 捕获错误并提示行号
来源：http://sat.tian-w.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://yng.andypj.xyz

[R34] 退出时清理
来源：http://jss.gogol.net.cn

trap 'rm -f "$tmp"' EXIT
来源：http://dad.9152youxi.cn

[R35] 后台执行并等待
来源：http://xmj.iojbl.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://jog.hfpthk.cn

[R36] 并发执行多个任务
来源：http://kjp.fktsv.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wtm.jqgufenzy.top

[R37] 把输出赋给变量
来源：http://vnq.gaohongyu789.top

files=$(ls -1)
来源：http://mst.yuxming.cn

[R38] 管道串联
来源：http://jal.jqgfzy.top

cat a.txt | grep -i error | wc -l
来源：http://mtb.nanxinkj.top

[R39] 重定向标准输出与错误
来源：http://jws.zhaomingkeji.xyz

cmd > out.log 2>&1
来源：http://psj.shanyushiyangkeji.top

[R40] 追加写日志
来源：http://avk.zhijiandao.cn

echo "log" >> out.log
来源：http://qai.quarkkingdee.top

[R41] 丢弃输出
来源：http://tvh.dashuyun.cn

cmd >/dev/null 2>&1
来源：http://iwl.nanxuanxn.top

[R42] 输入重定向
来源：http://mei.ppjwa.cn

wc -l < a.txt
来源：http://foi.sxryk.cn

[R43] 按名字查找文件
来源：http://chm.jinqigfzy.top

find . -name "*.log" -type f
来源：http://gkc.shanyushiyangkeji.top

[R44] 按修改时间查找
来源：http://nlw.shanyushiyangtech.top

find . -mtime -7 -type f
来源：http://nyx.zhongyouzk.top

[R45] 批量删除
来源：http://hpa.smart0.xyz

find . -name "*.tmp" -delete
来源：http://eni.zdqjudy.top

[R46] 递归替换文件内容
来源：http://tdg.ivvv.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://dhl.c1oappe.top

[R47] sed 单行替换
来源：http://drx.jinyuanbaomall.cn

sed -i 's/foo/bar/g' a.txt
来源：http://pjv.andypj.xyz

[R48] awk 取指定列
来源：http://gth.cucudq.cn

awk '{print $1, $3}' a.txt
来源：http://jjv.bbcook.cn

[R49] awk 带条件
来源：http://hki.bbcook.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://kll.ivvv.top

[R50] awk 求和
来源：http://qvl.mhx1999.top

awk '{s += $2} END {print s}' a.txt
来源：http://kii.gotoacloud.top

[R51] 排序去重取前几
来源：http://mey.tianlin.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://qhc.zhaomingkeji.xyz

[R52] 统计行数
来源：http://zdj.uphjek.com

wc -l a.txt
来源：http://nnz.jinghuilouyu.cn

[R53] 查看文件头与实时尾
来源：http://aba.dianchejie.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://eih.jlsjyb.cn

[R54] 比较两个文件
来源：http://ppu.quarkkingdee.top

diff a.txt b.txt
来源：http://pdn.cheryme.top

[R55] 压缩与解压
来源：http://dsw.hongshengwenyu.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wpc.quarkkingdee.top

[R56] 远程拷贝
来源：http://feo.daxiang520.top

scp file user@host:/path/
来源：http://uit.wangdashe.top

[R57] 远程执行命令
来源：http://vwd.xingfuxueyuan.xyz

ssh user@host 'uptime'
来源：http://acb.gogol.net.cn

[R58] 下载文件
来源：http://ndr.yonumen.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pfd.jqgfzy.top

[R59] 发 POST JSON
来源：http://kam.chenzaomai.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xxa.chenlongwang.top

[R60] 只看 HTTP 状态码
来源：http://sip.bjfxy.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pqg.hysaishi.cn

[R61] 磁盘占用
来源：http://juy.9152youxi.cn

df -h;  du -sh *
来源：http://skx.jiagoushi.top

[R62] 找最占空间的文件
来源：http://wsx.cheryme.top

du -ah . | sort -rh | head -10
来源：http://jcg.cdnleiting.top

[R63] 内存与进程
来源：http://adf.hfpthk.cn

free -h;  ps aux | grep nginx
来源：http://uxt.zhengqikj.top

[R64] 结束进程
来源：http://cws.guowangkeji.top

kill -9 $(pgrep -f app.py)
来源：http://skt.yuxming.cn

[R65] 查看端口占用
来源：http://grk.hesvh.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://uyr.ivvv.top

[R66] 定时任务
来源：http://sah.ppjwa.cn

crontab -e;  crontab -l
来源：http://kvm.tian-w.cn

[R67] 生成随机十六进制串
来源：http://bgf.gzhubu.top

openssl rand -hex 16
来源：http://prg.gaohongyu789.top

[R68] 计算文件校验值
来源：http://ycv.sysykeji.top

sha256sum a.txt;  md5sum a.txt
来源：http://evf.yvedp.cn

[R69] 生成随机密码
来源：http://nyi.shuidangran.top

head -c 16 /dev/urandom | base64
来源：http://zwo.guannengcc.top

[R70] 时间戳与互转
来源：http://eqy.guannengcc.top

date +%s;  date -d @1700000000
来源：http://mzm.fanxiaobao.xyz

[R71] 日期格式化
来源：http://mbc.epnwcf.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://bab.daxiang520.top

[R72] 等待端口就绪
来源：http://gov.zhijiandao.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://czy.cashguo.top

[R73] 分割大日志
来源：http://lwe.hammf.cn

split -l 1000 big.log part_
来源：http://mhp.fktsv.cn

[R74] 批量重命名
来源：http://ryl.wangshuangyany.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://tjr.shanyushiyangtech.top

[R75] 导出环境变量
来源：http://nhz.daria6918.cn

export PATH="$HOME/bin:$PATH"
来源：http://mzk.xziqi.cn

[R76] 使用临时文件
来源：http://auz.cdnleiting.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fnh.cashguo.top

[R77] 读取用户输入
来源：http://wnj.fanxiaobao.xyz

read -rp "请输入: " ans
来源：http://ocd.52xcode.cn

[R78] 交互式菜单
来源：http://jsq.ybcxt.top

select opt in a b c; do echo "$opt"; break; done
来源：http://zui.yj202588.top

[R79] 解析命令行选项
来源：http://pjd.cdnleiting.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kpq.jiagoushi.top

[R80] 查看脚本执行耗时
来源：http://qcg.bbcook.cn

time ./run.sh
来源：http://hbs.guannengcc.top

================================================================================
来源：http://nvj.yuanzhike.top

S. C / C++ 专题
来源：http://otn.0kj1m.cn

================================================================================
来源：http://qrg.tarul.cn

[S01] C：Hello World
来源：http://ayb.xziqi.cn

#include <stdio.h>
来源：http://kyr.zhijiandao.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jeo.zhoulong.xyz

[S02] C：变量与格式化输出
来源：http://eyx.ywan-chungtsiang.top

int a = 10; printf("%d\n", a);
来源：http://sqg.dashuyun.cn

[S03] C：读入整数
来源：http://ggd.haohaochexian.top

int x; scanf("%d", &x);
来源：http://igs.guannengcc.top

[S04] C：字符串复制
来源：http://wvs.hammf.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xgu.aizwys.cn

[S05] C：字符串长度
来源：http://uiq.nanxinkj.top

strlen(s)
来源：http://mgp.gotoacloud.top

[S06] C：字符串比较
来源：http://kvj.zhengqikj.top

strcmp(a, b) == 0
来源：http://jwf.sufxvd.cn

[S07] C：数组遍历求和
来源：http://kss.chenzaomai.com

for (int i = 0; i < n; i++) sum += a[i];
来源：http://lin.tian-w.cn

[S08] C：动态内存分配与释放
来源：http://nme.yj20258888.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tit.zhiwuduotai.top

[S09] C：结构体定义与初始化
来源：http://hlj.yuanzhike.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bzx.yj202588.top

[S10] C：指针与解引用
来源：http://xtn.vqdsnc.cn

int *p = &a;  *p = 5;
来源：http://kmt.havefunace.top

[S11] C：逐行读文件
来源：http://xnw.tianlin.xyz

FILE *f = fopen("a.txt", "r");
来源：http://hav.c1oappe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://qqs.fktsv.cn

fclose(f);
来源：http://tku.9152youxi.cn

[S12] C：写文件
来源：http://hlx.gogol.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yhh.uphjek.com

[S13] C：宏定义
来源：http://wwv.guowangkeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xvr.gotoacloud.top

[S14] C：枚举
来源：http://zct.birdmap.top

enum Color { RED, GREEN, BLUE };
来源：http://woj.nanxuanxn.top

[S15] C：类型转换
来源：http://mja.shzxlz.cn

(double) a / b
来源：http://yly.jianghu66.top

[S16] C：位操作置位
来源：http://etc.nwbrower.top

x |= (1 << 3);
来源：http://zdu.c1oappe.top

[S17] C：安全拼接字符串
来源：http://won.andypj.xyz

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xvx.sysykeji.top

[S18] C：命令行参数
来源：http://gfa.chenjidiqi.icu

int main(int argc, char **argv)
来源：http://jsc.sufxvd.cn

[S19] C：快速排序
来源：http://izn.wangdashe.top

qsort(a, n, sizeof(int), cmp);
来源：http://fgd.tarul.cn

[S20] C：二分查找
来源：http://ahh.316326.xyz

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nne.yj20258.top

[S21] C：字符类别判断
来源：http://zdb.yj20258.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://igm.iojbl.cn

[S22] C：字符串转数字
来源：http://azr.pycfn.com


<!-- 参考信息 -->