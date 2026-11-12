代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://pas.bjfxy.top

[Q54] 清空表
来源：http://vvx.wangdashe.top

TRUNCATE TABLE logs;
来源：http://bbr.ybcxt.top

[Q55] 排名（并列占位）
来源：http://bxc.mhx1999.top

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://yzo.zycfv.cn

[Q56] 密集排名（并列不占位）
来源：http://nhc.9152youxi.cn

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://bpo.jinghuilouyu.cn

[Q57] 行号
来源：http://wvn.vqdsnc.cn

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://abb.aibaodan.cn

[Q58] 累计求和
来源：http://tsm.cqqwz.cn

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://afb.pengpengdd.cyou

[Q59] 分组内累计
来源：http://fwp.cashguo.top

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ebf.chenlongwang.top

[Q60] 取上一行 / 下一行
来源：http://rou.hammf.cn

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://cnn.chenjidiqi.icu

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://dtc.gogol.net.cn

[Q61] 移动平均
来源：http://vhk.xylfe.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://jzh.pengpengdd.cyou

[Q62] 分组占比
来源：http://exm.smart0.xyz

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://zbh.52xcode.cn

[Q63] 开启事务
来源：http://war.gotoacloud.top

START TRANSACTION;                -- 或 BEGIN
来源：http://thy.cashguo.top

[Q64] 提交事务
来源：http://ogm.fengsongda.top

COMMIT;
来源：http://izw.cucudq.cn

[Q65] 回滚事务
来源：http://hpd.yangfankeji.com

ROLLBACK;
来源：http://vte.feifeiyinyue.top

[Q66] 行锁查询
来源：http://pbj.shuidangran.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://bzx.gogol.net.cn

[Q67] 设置隔离级别
来源：http://ogn.xylfe.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://xdg.zycfv.cn

[Q68] 保存点
来源：http://sab.yfazqb.com

SAVEPOINT sp1;
来源：http://klp.cdnleiting.top

ROLLBACK TO sp1;
来源：http://tye.hongshengwenyu.top

[Q69] 查看执行计划
来源：http://rmi.jinghuilouyu.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://ice.hcnkem.com

[Q70] 更新统计信息
来源：http://fbe.sweek.top

ANALYZE TABLE users;
来源：http://vmo.shzxlz.cn

[Q71] 查看建表语句
来源：http://ycq.nanxuanxn.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hnb.chenjidiqi.icu

[Q72] 查看索引
来源：http://isi.ctjpmb.com

SHOW INDEX FROM users;
来源：http://ous.zhijiandao.cn

[Q73] 查看表状态
来源：http://bog.uphjek.com

SHOW TABLE STATUS LIKE 'users';
来源：http://ytk.nwbrower.top

[Q74] 强制使用索引
来源：http://nzl.ybcxt.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://eiu.tianlin.xyz

[Q75] 日期格式化
来源：http://nbd.guowangkeji.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://skd.hfpthk.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uzj.gotoacloud.top

[Q76] 按天统计
来源：http://cjm.yj20258.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://lga.xingfuxueyuan.xyz

[Q77] 时间加减
来源：http://hnu.xinyue.icu

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://qtk.52xcode.cn

[Q78] 当前时间
来源：http://jou.zhaomingkeji.xyz

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://vbs.yj20258.top

[Q79] 字符串拼接
来源：http://ybi.vehdjk.com

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://rvl.jinghuilouyu.cn

[Q80] 字符串截取
来源：http://xcq.redwolf501.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://uiq.chenzaomai.com

[Q81] 字符串替换
来源：http://tpt.shanyushiyangtech.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hht.shzxlz.cn

[Q82] 字符长度与字节长度
来源：http://qln.ppjwa.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://onq.0kj1m.cn

[Q83] 大小写转换
来源：http://upp.cdnleiting.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://vec.nwbrower.top

[Q84] 去除首尾空格
来源：http://ieg.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://hxz.ppjwa.cn

[Q85] 数值取整
来源：http://nwy.cqqwz.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://qof.pengpengdd.cyou

[Q86] 读取 JSON 字段
来源：http://lsr.fktsv.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://pie.bbcook.cn

[Q87] JSON 字段做条件
来源：http://egk.shuidangran.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uxr.yanxiufei.cn

[Q88] 行转列（条件聚合）
来源：http://oyh.shanyushiyangtech.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://bki.tarul.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://yae.jinghuilouyu.cn

[Q89] 判断表是否存在
来源：http://unp.tarul.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://kdf.jlsjyb.cn

[Q90] 生成序号列
来源：http://iqc.wangshuangyany.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ilv.vqdsnc.cn

================================================================================
来源：http://gbp.pycfn.com

R. Bash 专题
来源：http://pzi.chenlongwang.top

================================================================================
来源：http://qgc.ehwqpu.com

[R01] shebang 与严格模式
来源：http://ury.svipenyu.cn

#!/usr/bin/env bash
来源：http://xtt.shangyingyoupin.top

set -euo pipefail
来源：http://wsu.jinqigfzy.top

[R02] 变量赋值与使用
来源：http://bcx.gaohongyu789.top

name="Tom"; echo "$name"
来源：http://qww.gogol.net.cn

[R03] 只读变量
来源：http://nyb.dashuyun.cn

readonly PI=3.14
来源：http://njr.xingfuxueyuan.xyz

[R04] 位置参数
来源：http://hqw.gaohongyu789.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://scl.yuxming.cn

[R05] 参数默认值
来源：http://uhq.yfazqb.com

name="${1:-default}"
来源：http://gey.hesvh.cn

[R06] 判断命令是否存在
来源：http://qli.kuanghao11.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://efp.tianlin.xyz

[R07] if 判断文件
来源：http://sqw.ybcxt.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://tfg.0kj1m.cn

[R08] 数值比较
来源：http://isi.snrcjt.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://euc.quarkkingdee.top

[R09] 字符串比较
来源：http://naw.xinyue.icu

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zjq.cheryme.top

[R10] 正则匹配
来源：http://hmp.jianghu66.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://orv.ehwqpu.com

[R11] case 多分支
来源：http://inr.gotoacloud.top

case "$1" in
来源：http://meq.kuanghao11.cn

start) echo "启动" ;;
来源：http://rsj.c1oappe.top

stop)  echo "停止" ;;
来源：http://bwa.dashuyun.cn

*)     echo "未知命令" ;;
来源：http://heh.bbcook.cn

esac
来源：http://dkk.shuidangran.top

[R12] for 遍历文件
来源：http://tnl.ivvv.top

for f in *.txt; do echo "$f"; done
来源：http://xoh.hesvh.cn

[R13] for 计数循环
来源：http://lwf.shuidangran.top

for i in {1..10}; do echo "$i"; done
来源：http://imx.shuidangran.top

[R14] C 风格 for
来源：http://axu.jinqigfzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://awm.yvedp.cn

[R15] while 逐行读文件
来源：http://euu.xinyue.icu

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://ujg.nwbrower.top

[R16] until 等待条件
来源：http://hbx.sjlbkw.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wlh.hammf.cn

[R17] 数组定义与取值
来源：http://kgg.cqqwz.cn

arr=(a b c); echo "${arr[0]}"
来源：http://kky.vqdsnc.cn

[R18] 遍历数组
来源：http://zjk.iojbl.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://fxe.sufxvd.cn

[R19] 数组长度
来源：http://cps.chenjidiqi.icu

echo "${#arr[@]}"
来源：http://xvk.snrcjt.cn

[R20] 关联数组（字典）
来源：http://kxr.ivvv.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qab.fzhhl.top

[R21] 字符串长度
来源：http://ons.ydjk.org.cn

echo "${#s}"
来源：http://cqb.ivvv.top

[R22] 截取子串
来源：http://gsy.iojbl.cn

echo "${s:0:5}"
来源：http://rad.ydzc1.top

[R23] 字符串替换
来源：http://sqy.zhongyouzk.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fri.yj20258888.top

[R24] 大小写转换
来源：http://bmf.yj20258.top

echo "${s^^}"; echo "${s,,}"
来源：http://nkz.shzxlz.cn

[R25] 去后缀 / 去前缀
来源：http://zjg.hfpthk.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://cid.cdnleiting.top

[R26] 命令替换
来源：http://bis.yfazqb.com

now=$(date +%F); echo "$now"
来源：http://blr.daxiang520.top

[R27] 算术展开
来源：http://vsv.zhoulong.xyz

echo $((1 + 2 * 3))
来源：http://vvc.cqqwz.cn

[R28] 浮点运算
来源：http://yqs.shzxlz.cn

echo "scale=2; 10/3" | bc
来源：http://hlx.feifeiyinyue.top

[R29] 定义函数
来源：http://wgw.yangfankeji.com

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mva.haohaochexian.top

[R30] 函数返回状态码
来源：http://cvh.yfazqb.com

f() { return 0; }; f || echo "失败了"
来源：http://bub.hywenlv.cn

[R31] 局部变量
来源：http://mgc.bbcook.cn

f() { local x=1; echo "$x"; }
来源：http://xjv.zdqjudy.top

[R32] 参数个数校验
来源：http://xvt.gzhubu.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://bgt.hnqzz.top

[R33] 捕获错误并提示行号
来源：http://ftx.hammf.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://tkt.vqdsnc.cn

[R34] 退出时清理
来源：http://hof.jianghu66.top

trap 'rm -f "$tmp"' EXIT
来源：http://qxx.guannengcc.top

[R35] 后台执行并等待
来源：http://tvy.smart0.xyz

sleep 5 & pid=$!; wait "$pid"
来源：http://ajc.zhiwuduotai.top

[R36] 并发执行多个任务
来源：http://bxx.zhaomingkeji.xyz

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://nfn.yangfankeji.com

[R37] 把输出赋给变量
来源：http://han.tarul.cn

files=$(ls -1)
来源：http://hvn.ivvv.top

[R38] 管道串联
来源：http://wym.gzhubu.top

cat a.txt | grep -i error | wc -l
来源：http://pvn.fktsv.cn

[R39] 重定向标准输出与错误
来源：http://kwh.chenjidiqi.icu

cmd > out.log 2>&1
来源：http://fec.gotoacloud.top

[R40] 追加写日志
来源：http://psc.yvedp.cn

echo "log" >> out.log
来源：http://hhm.mhx1999.top

[R41] 丢弃输出
来源：http://goq.chenlongwang.top

cmd >/dev/null 2>&1
来源：http://pov.ehwqpu.com

[R42] 输入重定向
来源：http://scg.redwolf501.top

wc -l < a.txt
来源：http://cyz.nanxuanxn.top

[R43] 按名字查找文件
来源：http://eiw.shuidangran.top

find . -name "*.log" -type f
来源：http://hkh.yj202588.top

[R44] 按修改时间查找
来源：http://ldd.c1oappe.top

find . -mtime -7 -type f
来源：http://ofr.fengsongda.top

[R45] 批量删除
来源：http://llk.ctjpmb.com

find . -name "*.tmp" -delete
来源：http://ikt.meibo888.top

[R46] 递归替换文件内容
来源：http://vnd.zhaomingkeji.xyz

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xta.kuanghao11.cn

[R47] sed 单行替换
来源：http://emp.shangyingyoupin.top

sed -i 's/foo/bar/g' a.txt
来源：http://swd.chenlongwang.top

[R48] awk 取指定列
来源：http://ofc.gogol.net.cn

awk '{print $1, $3}' a.txt
来源：http://eua.fanxiaobao.xyz

[R49] awk 带条件
来源：http://wsv.shanyushiyangkeji.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mde.aibaodan.cn

[R50] awk 求和
来源：http://est.vehdjk.com

awk '{s += $2} END {print s}' a.txt
来源：http://qmo.ehwqpu.com

[R51] 排序去重取前几
来源：http://gvy.vqdsnc.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://rle.ybcxt.top

[R52] 统计行数
来源：http://hfs.zdbjq.cn

wc -l a.txt
来源：http://hbq.xylfe.cn

[R53] 查看文件头与实时尾
来源：http://awj.epnwcf.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gjg.tarul.cn

[R54] 比较两个文件
来源：http://ryz.jinghuilouyu.cn

diff a.txt b.txt
来源：http://eoj.andypj.xyz

[R55] 压缩与解压
来源：http://osc.jiagoushi.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://iwl.svipenyu.cn

[R56] 远程拷贝
来源：http://bsu.zhiwuduotai.top

scp file user@host:/path/
来源：http://gwo.chenzaomai.com

[R57] 远程执行命令
来源：http://aru.yongpay.top

ssh user@host 'uptime'
来源：http://tsu.shuidangran.top

[R58] 下载文件
来源：http://bme.xuetiantiany.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://nfj.xuetiantiany.cn

[R59] 发 POST JSON
来源：http://wop.xziqi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://koo.zhengqikj.top

[R60] 只看 HTTP 状态码
来源：http://etm.sxryk.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://lfs.yongpay.top

[R61] 磁盘占用
来源：http://whg.hnqzz.top

df -h;  du -sh *
来源：http://kid.xingfuxueyuan.xyz

[R62] 找最占空间的文件
来源：http://mch.xziqi.cn

du -ah . | sort -rh | head -10
来源：http://jtq.bjfxy.top

[R63] 内存与进程
来源：http://qfi.ybcxt.top

free -h;  ps aux | grep nginx
来源：http://vas.ehwqpu.com

[R64] 结束进程
来源：http://gdf.zhaomingkeji.xyz

kill -9 $(pgrep -f app.py)
来源：http://tef.iojbl.cn

[R65] 查看端口占用
来源：http://vgq.fktsv.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ryl.yonumen.top

[R66] 定时任务
来源：http://vhy.bjfxy.top

crontab -e;  crontab -l
来源：http://cjn.nanxuanxn.top

[R67] 生成随机十六进制串
来源：http://fwh.chenlongwang.top

openssl rand -hex 16
来源：http://rxb.pycfn.com

[R68] 计算文件校验值
来源：http://wwz.daria6918.cn

sha256sum a.txt;  md5sum a.txt
来源：http://dfu.yvedp.cn

[R69] 生成随机密码
来源：http://xkc.shanyushiyangtech.top

head -c 16 /dev/urandom | base64
来源：http://jur.jyoumei.cn

[R70] 时间戳与互转
来源：http://oru.guannengcc.top

date +%s;  date -d @1700000000
来源：http://rxd.c1oappe.top

[R71] 日期格式化
来源：http://yqa.ehwqpu.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://vvv.quarkkingdee.top

[R72] 等待端口就绪
来源：http://zzp.tianlin.xyz

until nc -z localhost 3306; do sleep 1; done
来源：http://lme.gotoacloud.top

[R73] 分割大日志
来源：http://nme.tarul.cn

split -l 1000 big.log part_
来源：http://ptf.xylfe.cn

[R74] 批量重命名
来源：http://adh.zdqjudy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qmz.fanxiaobao.xyz

[R75] 导出环境变量
来源：http://nxr.yonumen.top

export PATH="$HOME/bin:$PATH"
来源：http://bgi.yvedp.cn

[R76] 使用临时文件
来源：http://qam.chenzaomai.com

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lqw.jinghuilouyu.cn

[R77] 读取用户输入
来源：http://rso.ydjk.org.cn

read -rp "请输入: " ans
来源：http://oga.havefunace.top

[R78] 交互式菜单
来源：http://byk.hcnkem.com

select opt in a b c; do echo "$opt"; break; done
来源：http://kpc.yj20258.top

[R79] 解析命令行选项
来源：http://xju.zhijiandao.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://eap.gogol.net.cn

[R80] 查看脚本执行耗时
来源：http://pqh.yj20258888.top

time ./run.sh
来源：http://van.9152youxi.cn

================================================================================
来源：http://odp.bjfxy.top

S. C / C++ 专题
来源：http://wbn.9152youxi.cn

================================================================================
来源：http://mzl.quarkkingdee.top

[S01] C：Hello World
来源：http://wxu.hnxiangtu.top

#include <stdio.h>
来源：http://ziw.zhengqikj.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://vyg.jianghu66.top

[S02] C：变量与格式化输出
来源：http://uep.tian-w.cn

int a = 10; printf("%d\n", a);
来源：http://mdr.iojbl.cn

[S03] C：读入整数
来源：http://ual.yj20258888.top

int x; scanf("%d", &x);
来源：http://hth.hnxiangtu.top

[S04] C：字符串复制
来源：http://mcg.9152youxi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cyx.jqgfzy.top

[S05] C：字符串长度
来源：http://bqh.cqqwz.cn

strlen(s)
来源：http://rti.jinyuanbaomall.cn

[S06] C：字符串比较
来源：http://lps.redwolf501.top

strcmp(a, b) == 0
来源：http://chx.epnwcf.com

[S07] C：数组遍历求和
来源：http://hay.hywenlv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sbx.wangdashe.top

[S08] C：动态内存分配与释放
来源：http://zjl.feifeiyinyue.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lkk.cqqwz.cn

[S09] C：结构体定义与初始化
来源：http://glg.zhaomingkeji.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ilk.yvedp.cn

[S10] C：指针与解引用
来源：http://pks.xuanzx.com

int *p = &a;  *p = 5;
来源：http://lqf.fzhhl.top

[S11] C：逐行读文件
来源：http://iut.bjfxy.top

FILE *f = fopen("a.txt", "r");
来源：http://ezc.zhongyouzk.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://pum.shuidangran.top

fclose(f);
来源：http://gyj.xziqi.cn

[S12] C：写文件
来源：http://qju.havefunace.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wtf.ivvv.top

[S13] C：宏定义
来源：http://zdo.fanxiaobao.xyz

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cbq.sxryk.cn

[S14] C：枚举
来源：http://wka.fzhhl.top

enum Color { RED, GREEN, BLUE };
来源：http://sys.wangdashe.top

[S15] C：类型转换
来源：http://nao.zdbjq.cn

(double) a / b
来源：http://kti.cheryme.top

[S16] C：位操作置位
来源：http://jva.dashuyun.cn

x |= (1 << 3);
来源：http://gkb.kuanghao11.cn

[S17] C：安全拼接字符串
来源：http://kow.zhongyouzk.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ofo.zhengqikj.top

[S18] C：命令行参数
来源：http://byb.ppjwa.cn

int main(int argc, char **argv)
来源：http://pxv.svipenyu.cn

[S19] C：快速排序
来源：http://ibd.tian-w.cn

qsort(a, n, sizeof(int), cmp);
来源：http://hzj.daria6918.cn

[S20] C：二分查找
来源：http://sym.tian-w.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ace.andypj.xyz

[S21] C：字符类别判断
来源：http://bij.jinqigfzy.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wrb.jianghu66.top

[S22] C：字符串转数字
来源：http://bap.xinyue.icu

atoi("42");  strtod("3.14", NULL);
来源：http://bgl.hywenlv.cn

[S23] C：随机数
来源：http://gwd.uphjek.com

srand(time(NULL));  int r = rand() % 100;
来源：http://enh.iojbl.cn

[S24] C：获取本地时间
来源：http://bns.hnqzz.top


<!-- 参考信息 -->