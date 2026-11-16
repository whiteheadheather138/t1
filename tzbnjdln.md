代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://uiz.yj20258.top

[Q54] 清空表
来源：http://dhm.jlsjyb.cn

TRUNCATE TABLE logs;
来源：http://ytc.cdnleiting.top

[Q55] 排名（并列占位）
来源：http://mcu.jyoumei.cn

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://qpe.yfazqb.com

[Q56] 密集排名（并列不占位）
来源：http://evp.yj202588.top

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://qsz.uphjek.com

[Q57] 行号
来源：http://lyf.nwbrower.top

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://axm.tianlin.xyz

[Q58] 累计求和
来源：http://isp.zhiwuduotai.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://bwe.jinyuanbaomall.cn

[Q59] 分组内累计
来源：http://rxv.tian-w.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://pnv.yonumen.top

[Q60] 取上一行 / 下一行
来源：http://axo.shanyushiyangtech.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://sat.jianghu66.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://zxd.fengsongda.top

[Q61] 移动平均
来源：http://rrb.zhiwuduotai.top

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://yeb.tian-w.cn

[Q62] 分组占比
来源：http://dpy.tanke756.top

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://asd.yueranfly.top

[Q63] 开启事务
来源：http://qrb.hywenlv.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://lwd.jqgfzy.top

[Q64] 提交事务
来源：http://oth.cqqwz.cn

COMMIT;
来源：http://niv.hnxiangtu.top

[Q65] 回滚事务
来源：http://gev.ctjpmb.com

ROLLBACK;
来源：http://nqa.zhoulong.xyz

[Q66] 行锁查询
来源：http://lmc.yj20258.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://eiy.xylfe.cn

[Q67] 设置隔离级别
来源：http://avd.jiagoushi.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://tvt.shuidangran.top

[Q68] 保存点
来源：http://bti.tianlin.xyz

SAVEPOINT sp1;
来源：http://rpq.tanke756.top

ROLLBACK TO sp1;
来源：http://yow.bjfxy.top

[Q69] 查看执行计划
来源：http://eoc.uphjek.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://tua.nanxinkj.top

[Q70] 更新统计信息
来源：http://vhz.zdqjudy.top

ANALYZE TABLE users;
来源：http://qnj.jiagoushi.top

[Q71] 查看建表语句
来源：http://hzc.gogol.net.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://iin.gogol.net.cn

[Q72] 查看索引
来源：http://qzc.daxiang520.top

SHOW INDEX FROM users;
来源：http://xhj.hammf.cn

[Q73] 查看表状态
来源：http://cwi.ctjpmb.com

SHOW TABLE STATUS LIKE 'users';
来源：http://fie.hcnkem.com

[Q74] 强制使用索引
来源：http://wqd.yanxiufei.cn

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://svd.hongshengwenyu.top

[Q75] 日期格式化
来源：http://uez.c1oappe.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wbu.fengsongda.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ffv.jinyuanbaomall.cn

[Q76] 按天统计
来源：http://hbh.cheryme.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://kax.zhijiandao.cn

[Q77] 时间加减
来源：http://nul.chenzaomai.com

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://die.xinyue.icu

[Q78] 当前时间
来源：http://vdj.wangshuangyany.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://jxw.pengpengdd.cyou

[Q79] 字符串拼接
来源：http://czg.hnqzz.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://gkl.pycfn.com

[Q80] 字符串截取
来源：http://udz.sysykeji.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://lih.pycfn.com

[Q81] 字符串替换
来源：http://ygm.cqqwz.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rnp.redwolf501.top

[Q82] 字符长度与字节长度
来源：http://wpw.ybcxt.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://isp.ydzc1.top

[Q83] 大小写转换
来源：http://qex.zhixingplan.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wza.guowangkeji.top

[Q84] 去除首尾空格
来源：http://xyc.bbcook.cn

SELECT TRIM(name) FROM users;
来源：http://ufl.nanxuanxn.top

[Q85] 数值取整
来源：http://gyc.c1oappe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://zfp.jinqigufen.top

[Q86] 读取 JSON 字段
来源：http://llz.yonumen.top

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wiv.redwolf501.top

[Q87] JSON 字段做条件
来源：http://pfl.yj20258.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://xjd.havefunace.top

[Q88] 行转列（条件聚合）
来源：http://upp.aibaodan.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://ojb.dianchejie.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mig.jiagoushi.top

[Q89] 判断表是否存在
来源：http://tys.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hbi.yuxming.cn

[Q90] 生成序号列
来源：http://ovk.yanxiufei.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ayg.shuidangran.top

================================================================================
来源：http://nom.zhoulong.xyz

R. Bash 专题
来源：http://nyo.svipenyu.cn

================================================================================
来源：http://dyp.hnxiangtu.top

[R01] shebang 与严格模式
来源：http://nxw.yuxming.cn

#!/usr/bin/env bash
来源：http://wgp.xuetiantiany.cn

set -euo pipefail
来源：http://dfj.316326.xyz

[R02] 变量赋值与使用
来源：http://lms.jinqigfzy.top

name="Tom"; echo "$name"
来源：http://yxc.fanxiaobao.xyz

[R03] 只读变量
来源：http://eoz.ydzc1.top

readonly PI=3.14
来源：http://zmk.zdqjudy.top

[R04] 位置参数
来源：http://lyg.jlsjyb.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://ykh.52xcode.cn

[R05] 参数默认值
来源：http://ngw.cqqwz.cn

name="${1:-default}"
来源：http://ilg.meibo888.top

[R06] 判断命令是否存在
来源：http://xnq.cdnleiting.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://yhn.tianlin.xyz

[R07] if 判断文件
来源：http://mcr.jinqigufen.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wvv.bjfxy.top

[R08] 数值比较
来源：http://zsb.cqqwz.cn

if (( a > b )); then echo "a 更大"; fi
来源：http://vft.hcnkem.com

[R09] 字符串比较
来源：http://eud.havefunace.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://sqy.zhaomingkeji.xyz

[R10] 正则匹配
来源：http://bqi.cdnleiting.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://bmz.0kj1m.cn

[R11] case 多分支
来源：http://kut.jiagoushi.top

case "$1" in
来源：http://ppz.guowangkeji.top

start) echo "启动" ;;
来源：http://fvd.fanxiaobao.xyz

stop)  echo "停止" ;;
来源：http://uqv.yangfankeji.com

*)     echo "未知命令" ;;
来源：http://iik.xingfuxueyuan.xyz

esac
来源：http://sha.ydjk.org.cn

[R12] for 遍历文件
来源：http://ajv.zycfv.cn

for f in *.txt; do echo "$f"; done
来源：http://xcw.52xcode.cn

[R13] for 计数循环
来源：http://kpn.shangyingyoupin.top

for i in {1..10}; do echo "$i"; done
来源：http://spf.svipenyu.cn

[R14] C 风格 for
来源：http://new.cucudq.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://qso.pengpengdd.cyou

[R15] while 逐行读文件
来源：http://rwv.tian-w.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://pis.gogol.net.cn

[R16] until 等待条件
来源：http://etl.hcnkem.com

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hhm.svipenyu.cn

[R17] 数组定义与取值
来源：http://dhl.yuanzhike.top

arr=(a b c); echo "${arr[0]}"
来源：http://kqt.fehbvm.com

[R18] 遍历数组
来源：http://fme.fengsongda.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://rtk.vqdsnc.cn

[R19] 数组长度
来源：http://spe.tanke756.top

echo "${#arr[@]}"
来源：http://vyf.gaohongyu789.top

[R20] 关联数组（字典）
来源：http://etd.fktsv.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://kda.xziqi.cn

[R21] 字符串长度
来源：http://kkw.yonumen.top

echo "${#s}"
来源：http://agi.bjfxy.top

[R22] 截取子串
来源：http://yqx.hysaishi.cn

echo "${s:0:5}"
来源：http://zct.epnwcf.com

[R23] 字符串替换
来源：http://cye.yfazqb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://vty.sufxvd.cn

[R24] 大小写转换
来源：http://ivg.yuxming.cn

echo "${s^^}"; echo "${s,,}"
来源：http://itq.jqgufenzy.top

[R25] 去后缀 / 去前缀
来源：http://hyb.guowangkeji.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://blp.fanxiaobao.xyz

[R26] 命令替换
来源：http://xcc.cucudq.cn

now=$(date +%F); echo "$now"
来源：http://vkl.shanyushiyangkeji.top

[R27] 算术展开
来源：http://gky.sjlbkw.cn

echo $((1 + 2 * 3))
来源：http://gcs.yuxming.cn

[R28] 浮点运算
来源：http://cif.zhaomingkeji.xyz

echo "scale=2; 10/3" | bc
来源：http://cez.dashuyun.cn

[R29] 定义函数
来源：http://ntk.cqqwz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://qdk.zhengqikj.top

[R30] 函数返回状态码
来源：http://hqn.jinqigufen.top

f() { return 0; }; f || echo "失败了"
来源：http://sol.daxiang520.top

[R31] 局部变量
来源：http://rwu.pycfn.com

f() { local x=1; echo "$x"; }
来源：http://wrd.jqgfzy.top

[R32] 参数个数校验
来源：http://zwd.zhengqikj.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://elz.shanyushiyangtech.top

[R33] 捕获错误并提示行号
来源：http://ksl.birdmap.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://jyx.hysaishi.cn

[R34] 退出时清理
来源：http://dtd.svipenyu.cn

trap 'rm -f "$tmp"' EXIT
来源：http://tet.aibaodan.cn

[R35] 后台执行并等待
来源：http://rih.sjlbkw.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://pad.xylfe.cn

[R36] 并发执行多个任务
来源：http://fok.yfazqb.com

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://tpd.cdnleiting.top

[R37] 把输出赋给变量
来源：http://ggs.guowangkeji.top

files=$(ls -1)
来源：http://qcv.yj20258.top

[R38] 管道串联
来源：http://mzw.fanxiaobao.xyz

cat a.txt | grep -i error | wc -l
来源：http://gkl.hnxiangtu.top

[R39] 重定向标准输出与错误
来源：http://tyh.vehdjk.com

cmd > out.log 2>&1
来源：http://vkl.epnwcf.com

[R40] 追加写日志
来源：http://fyh.ivvv.top

echo "log" >> out.log
来源：http://loz.yongpay.top

[R41] 丢弃输出
来源：http://mff.kuanghao11.cn

cmd >/dev/null 2>&1
来源：http://afm.bjfxy.top

[R42] 输入重定向
来源：http://hhu.jqgfzy.top

wc -l < a.txt
来源：http://adm.vehdjk.com

[R43] 按名字查找文件
来源：http://ajr.jinqigfzy.top

find . -name "*.log" -type f
来源：http://who.nwbrower.top

[R44] 按修改时间查找
来源：http://fin.tianlin.xyz

find . -mtime -7 -type f
来源：http://rwz.zhixingplan.top

[R45] 批量删除
来源：http://hpm.haohaochexian.top

find . -name "*.tmp" -delete
来源：http://zsu.yj202588.top

[R46] 递归替换文件内容
来源：http://cee.jlsjyb.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mdc.jiagoushi.top

[R47] sed 单行替换
来源：http://ouq.kuanghao11.cn

sed -i 's/foo/bar/g' a.txt
来源：http://mwh.yueranfly.top

[R48] awk 取指定列
来源：http://bjo.gzhubu.top

awk '{print $1, $3}' a.txt
来源：http://rxm.kuanghao11.cn

[R49] awk 带条件
来源：http://yka.iojbl.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://eez.xylfe.cn

[R50] awk 求和
来源：http://mwm.zhijiandao.cn

awk '{s += $2} END {print s}' a.txt
来源：http://mom.svipenyu.cn

[R51] 排序去重取前几
来源：http://wfl.gaohongyu789.top

sort a.txt | uniq -c | sort -rn | head
来源：http://vgx.guannengcc.top

[R52] 统计行数
来源：http://qns.zhijiandao.cn

wc -l a.txt
来源：http://fvx.ehwqpu.com

[R53] 查看文件头与实时尾
来源：http://wzl.jqgufenzy.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://fwp.zhoulong.xyz

[R54] 比较两个文件
来源：http://lnf.fktsv.cn

diff a.txt b.txt
来源：http://fhk.pengpengdd.cyou

[R55] 压缩与解压
来源：http://ckp.wangshuangyany.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bqt.zdbjq.cn

[R56] 远程拷贝
来源：http://hpv.jianghu66.top

scp file user@host:/path/
来源：http://dfz.hammf.cn

[R57] 远程执行命令
来源：http://ksx.ydzc1.top

ssh user@host 'uptime'
来源：http://nuo.xingfuxueyuan.xyz

[R58] 下载文件
来源：http://awx.jianghu66.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gdf.chenjidiqi.icu

[R59] 发 POST JSON
来源：http://jhw.redwolf501.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://efc.fehbvm.com

[R60] 只看 HTTP 状态码
来源：http://onh.jinyuanbaomall.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ley.hcnkem.com

[R61] 磁盘占用
来源：http://cqc.yj20258888.top

df -h;  du -sh *
来源：http://hgh.gzhubu.top

[R62] 找最占空间的文件
来源：http://lqz.wangdashe.top

du -ah . | sort -rh | head -10
来源：http://ssp.nwbrower.top

[R63] 内存与进程
来源：http://vjd.chenjidiqi.icu

free -h;  ps aux | grep nginx
来源：http://rip.dashuyun.cn

[R64] 结束进程
来源：http://vnv.birdmap.top

kill -9 $(pgrep -f app.py)
来源：http://eov.jinqigufen.top

[R65] 查看端口占用
来源：http://drc.ehwqpu.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fba.ppjwa.cn

[R66] 定时任务
来源：http://egh.zdbjq.cn

crontab -e;  crontab -l
来源：http://rfl.aibaodan.cn

[R67] 生成随机十六进制串
来源：http://jbz.fengsongda.top

openssl rand -hex 16
来源：http://uhz.yfazqb.com

[R68] 计算文件校验值
来源：http://jff.fanxiaobao.xyz

sha256sum a.txt;  md5sum a.txt
来源：http://bhz.yj20258888.top

[R69] 生成随机密码
来源：http://nmn.hongshengwenyu.top

head -c 16 /dev/urandom | base64
来源：http://emg.ybcxt.top

[R70] 时间戳与互转
来源：http://pdk.hcnkem.com

date +%s;  date -d @1700000000
来源：http://wql.jianghu66.top

[R71] 日期格式化
来源：http://rcs.tianlin.xyz

date +"%Y-%m-%d %H:%M:%S"
来源：http://oun.wangshuangyany.cn

[R72] 等待端口就绪
来源：http://pes.hnxiangtu.top

until nc -z localhost 3306; do sleep 1; done
来源：http://xxf.zhijiandao.cn

[R73] 分割大日志
来源：http://ren.uphjek.com

split -l 1000 big.log part_
来源：http://ttl.52xcode.cn

[R74] 批量重命名
来源：http://keo.vqdsnc.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://phd.cashguo.top

[R75] 导出环境变量
来源：http://rck.yfazqb.com

export PATH="$HOME/bin:$PATH"
来源：http://pzo.fehbvm.com

[R76] 使用临时文件
来源：http://tpj.hnqzz.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xkj.xylfe.cn

[R77] 读取用户输入
来源：http://uth.ctjpmb.com

read -rp "请输入: " ans
来源：http://lql.chenlongwang.top

[R78] 交互式菜单
来源：http://cub.epnwcf.com

select opt in a b c; do echo "$opt"; break; done
来源：http://pxq.tanke756.top

[R79] 解析命令行选项
来源：http://iqc.iojbl.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jfb.tian-w.cn

[R80] 查看脚本执行耗时
来源：http://ngt.wangshuangyany.cn

time ./run.sh
来源：http://sxn.dashuyun.cn

================================================================================
来源：http://euf.52xcode.cn

S. C / C++ 专题
来源：http://lvx.jinqigfzy.top

================================================================================
来源：http://qvp.zhongyouzk.top

[S01] C：Hello World
来源：http://kjb.sysykeji.top

#include <stdio.h>
来源：http://gee.vehdjk.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://yrc.jlsjyb.cn

[S02] C：变量与格式化输出
来源：http://pts.yuxming.cn

int a = 10; printf("%d\n", a);
来源：http://foa.hammf.cn

[S03] C：读入整数
来源：http://bux.yongpay.top

int x; scanf("%d", &x);
来源：http://ckt.redwolf501.top

[S04] C：字符串复制
来源：http://qfz.fktsv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rdy.ctjpmb.com

[S05] C：字符串长度
来源：http://rpa.fengsongda.top

strlen(s)
来源：http://ouf.yuanzhike.top

[S06] C：字符串比较
来源：http://jwo.nanxinkj.top

strcmp(a, b) == 0
来源：http://twg.jiagoushi.top

[S07] C：数组遍历求和
来源：http://xdj.nanxuanxn.top

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ynu.shuidangran.top

[S08] C：动态内存分配与释放
来源：http://qeo.shanyushiyangtech.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pxu.bjfxy.top

[S09] C：结构体定义与初始化
来源：http://dlj.tianlin.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://usc.bjfxy.top

[S10] C：指针与解引用
来源：http://wge.jinqigufen.top

int *p = &a;  *p = 5;
来源：http://ncr.hysaishi.cn

[S11] C：逐行读文件
来源：http://iyx.shanyushiyangtech.top

FILE *f = fopen("a.txt", "r");
来源：http://iyc.fktsv.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://uzd.xziqi.cn

fclose(f);
来源：http://ofi.316326.xyz

[S12] C：写文件
来源：http://iny.ywan-chungtsiang.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qlz.xziqi.cn

[S13] C：宏定义
来源：http://zta.fehbvm.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://leb.hammf.cn

[S14] C：枚举
来源：http://nah.ybcxt.top

enum Color { RED, GREEN, BLUE };
来源：http://voy.svipenyu.cn

[S15] C：类型转换
来源：http://eap.fktsv.cn

(double) a / b
来源：http://xhb.xylfe.cn

[S16] C：位操作置位
来源：http://eaf.guannengcc.top

x |= (1 << 3);
来源：http://tvt.sweek.top

[S17] C：安全拼接字符串
来源：http://tnm.sjlbkw.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nbi.yanxiufei.cn

[S18] C：命令行参数
来源：http://fxo.yongpay.top

int main(int argc, char **argv)
来源：http://tqn.nwbrower.top

[S19] C：快速排序
来源：http://knn.hysaishi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sfs.havefunace.top

[S20] C：二分查找
来源：http://nqm.tian-w.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jdv.zdbjq.cn

[S21] C：字符类别判断
来源：http://lcn.xziqi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xgh.chenzaomai.com

[S22] C：字符串转数字
来源：http://haz.zhixingplan.top

atoi("42");  strtod("3.14", NULL);
来源：http://zkd.bjfxy.top

[S23] C：随机数
来源：http://dpw.feifeiyinyue.top

srand(time(NULL));  int r = rand() % 100;
来源：http://vve.fzhhl.top

[S24] C：获取本地时间
来源：http://xzi.zhaomingkeji.xyz


<!-- 参考信息 -->